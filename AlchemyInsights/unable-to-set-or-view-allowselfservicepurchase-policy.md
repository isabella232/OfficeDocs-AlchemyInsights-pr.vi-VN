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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091790"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="8d028-102">Không thể thiết lập hoặc xem chính sách AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="8d028-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="8d028-103">Khi cố gắng thiết lập hoặc xem chính sách AllowSelfServicePurchase, bạn nhận được thông báo lỗi sau:</span><span class="sxs-lookup"><span data-stu-id="8d028-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="8d028-104">*HandleError: không thể truy xuất chính sách sản phẩm với PolicyId ' AllowSelfServicePurchase ', ErrorMessage-kết nối cơ bản bị đóng: một lỗi không mong muốn xảy ra trên một gửi.*</span><span class="sxs-lookup"><span data-stu-id="8d028-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="8d028-105">Điều này có thể là do một phiên bản cũ hơn của Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="8d028-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="8d028-106">Để kết nối dịch vụ MSCommerce, bạn cần phải sử dụng TLS 1,2 hoặc cao hơn.</span><span class="sxs-lookup"><span data-stu-id="8d028-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="8d028-107">Hãy thử các bước sau để bật/đặt giao thức TLS 1,2, xác minh và thử lại.</span><span class="sxs-lookup"><span data-stu-id="8d028-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="8d028-108">Tại dấu nhắc lệnh PowerShell (PS C:\) nhập lệnh sau để đặt giao thức TLS phiên bản 1,2:</span><span class="sxs-lookup"><span data-stu-id="8d028-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="8d028-109">\[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="8d028-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="8d028-110">Kiểm tra giao thức TLS (s) sử dụng, với các lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="8d028-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="8d028-111">\[Net. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="8d028-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="8d028-112">Thử lại lệnh nhận hoặc Cập Nhật khi cần thiết.</span><span class="sxs-lookup"><span data-stu-id="8d028-112">Retry the Get or Update commands as needed.</span></span>

