---
title: Không thể đặt hoặc xem chính sách mua mua của allowselfservice
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735221"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9fecd-102">Không thể đặt hoặc xem chính sách mua mua của allowselfservice</span><span class="sxs-lookup"><span data-stu-id="9fecd-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9fecd-103">Khi cố gắng đặt hoặc xem chính sách mua mua của Allowselfservice, bạn nhận được thông báo lỗi sau đây:</span><span class="sxs-lookup"><span data-stu-id="9fecd-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9fecd-104">*HandleError: không thể truy xuất chính sách sản phẩm với nội dung mua ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ sở đã được đóng: một lỗi không mong muốn xảy ra khi gửi.*</span><span class="sxs-lookup"><span data-stu-id="9fecd-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9fecd-105">Điều này có thể do một phiên bản cũ của bảo mật tầng giao thông (TLS).</span><span class="sxs-lookup"><span data-stu-id="9fecd-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9fecd-106">Để kết nối với dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.</span><span class="sxs-lookup"><span data-stu-id="9fecd-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9fecd-107">Hãy thử các bước sau đây để bật/đặt giao thức TLS sang 1,2, xác nhận và thử lại.</span><span class="sxs-lookup"><span data-stu-id="9fecd-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9fecd-108">Tại dấu nhắc lệnh PowerShell (PS C: \) nhập lệnh sau đây để đặt giao thức TLS sang phiên bản 1,2:</span><span class="sxs-lookup"><span data-stu-id="9fecd-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="9fecd-109">Xác minh (các) (các) (các) (các) (các) (các) (các) (các) giao thức</span><span class="sxs-lookup"><span data-stu-id="9fecd-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="9fecd-110">Thử lại các lệnh tải xuống và Cập Nhật khi cần thiết.</span><span class="sxs-lookup"><span data-stu-id="9fecd-110">Retry the Get or Update commands as needed.</span></span>

