---
title: Tự dịch vụ mua PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091789"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="4dd23-102">Tự dịch vụ mua PowerShell</span><span class="sxs-lookup"><span data-stu-id="4dd23-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="4dd23-103">Để sử dụng mô-đun MSCommerce PowerShell, bạn cần cài đặt trên thiết bị Windows 10 với TLS 1,2 (quyền quản trị viên cục bộ cần thiết).</span><span class="sxs-lookup"><span data-stu-id="4dd23-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="4dd23-104">Nhập và kết nối với mô-đun MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="4dd23-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="4dd23-105">Khi được nhắc đăng nhập, bạn sẽ cần sử dụng thông tin đăng nhập vai trò quản trị viên toàn cầu hoặc thanh toán.</span><span class="sxs-lookup"><span data-stu-id="4dd23-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="4dd23-106">Nếu bạn không có TLS 1,2, bạn có thể nhận được lỗi sau khi cố gắng để có được hoặc cập nhật chính sách:</span><span class="sxs-lookup"><span data-stu-id="4dd23-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="4dd23-107">*ErrorMessage-kết nối cơ bản đã bị đóng: một lỗi không mong muốn xảy ra trên một gửi*.</span><span class="sxs-lookup"><span data-stu-id="4dd23-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



