---
title: Không thể đặt hoặc xem chính sách mua mua của allowselfservice
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826113"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="56e3c-102">Không thể đặt hoặc xem chính sách mua mua của allowselfservice</span><span class="sxs-lookup"><span data-stu-id="56e3c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="56e3c-103">Khi cố gắng đặt hoặc xem chính sách mua mua của Allowselfservice, bạn nhận được thông báo lỗi sau đây:</span><span class="sxs-lookup"><span data-stu-id="56e3c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="56e3c-104">*HandleError: không thể truy xuất chính sách sản phẩm với nội dung mua ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ sở đã được đóng: một lỗi không mong muốn xảy ra khi gửi.*</span><span class="sxs-lookup"><span data-stu-id="56e3c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="56e3c-105">Điều này có thể do một phiên bản cũ của bảo mật tầng giao thông (TLS).</span><span class="sxs-lookup"><span data-stu-id="56e3c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="56e3c-106">Để kết nối với dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.</span><span class="sxs-lookup"><span data-stu-id="56e3c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="56e3c-107">Hãy thử các bước sau đây để bật/đặt giao thức TLS sang 1,2, xác nhận và thử lại.</span><span class="sxs-lookup"><span data-stu-id="56e3c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="56e3c-108">Tại dấu nhắc lệnh PowerShell (PS C: \) nhập lệnh sau đây để đặt giao thức TLS sang phiên bản 1,2:</span><span class="sxs-lookup"><span data-stu-id="56e3c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="56e3c-109">Xác minh (các) (các) (các) (các) (các) (các) (các) (các) giao thức</span><span class="sxs-lookup"><span data-stu-id="56e3c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="56e3c-110">Thử lại các lệnh tải xuống và Cập Nhật khi cần thiết.</span><span class="sxs-lookup"><span data-stu-id="56e3c-110">Retry the Get or Update commands as needed.</span></span>

