---
title: Không thể thiết lập hoặc xem chính sách AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158583"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="fa503-102">Không thể thiết lập hoặc xem chính sách AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="fa503-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="fa503-103">Khi cố gắng thiết lập hoặc xem chính sách AllowSelfServicePurchase, bạn nhận được thông báo lỗi sau:</span><span class="sxs-lookup"><span data-stu-id="fa503-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="fa503-104">*HandleError: không thể truy xuất chính sách sản phẩm với PolicyId ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ bản bị đóng: một lỗi không mong muốn xảy ra trên một gửi.*</span><span class="sxs-lookup"><span data-stu-id="fa503-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="fa503-105">Điều này có thể là do một phiên bản cũ hơn của Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="fa503-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="fa503-106">Để kết nối dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.</span><span class="sxs-lookup"><span data-stu-id="fa503-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="fa503-107">Hãy thử các bước sau để bật/đặt giao thức TLS 1,2, xác minh và thử lại.</span><span class="sxs-lookup"><span data-stu-id="fa503-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="fa503-108">Tại dấu nhắc lệnh PowerShell (PS C:\) nhập lệnh sau để đặt giao thức TLS phiên bản 1,2:</span><span class="sxs-lookup"><span data-stu-id="fa503-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="fa503-109">Kiểm tra giao thức TLS (s) sử dụng, với các lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="fa503-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="fa503-110">Thử lại lệnh nhận hoặc Cập Nhật khi cần thiết.</span><span class="sxs-lookup"><span data-stu-id="fa503-110">Retry the Get or Update commands as needed.</span></span>

