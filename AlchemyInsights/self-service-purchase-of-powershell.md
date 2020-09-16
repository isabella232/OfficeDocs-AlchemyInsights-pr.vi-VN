---
title: Mua tự phục vụ cho PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740020"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="1f5cc-102">Mua tự phục vụ cho PowerShell</span><span class="sxs-lookup"><span data-stu-id="1f5cc-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="1f5cc-103">Để sử dụng mô-đun MSCommerce PowerShell, bạn cần cài đặt nó trên một thiết bị chạy Windows 10 với TLS 1,2 (quyền của người quản trị cục bộ).</span><span class="sxs-lookup"><span data-stu-id="1f5cc-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="1f5cc-104">Nhập và kết nối với mô-đun MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="1f5cc-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="1f5cc-105">Khi được nhắc đăng nhập, bạn sẽ cần sử dụng thông tin xác thực vai trò người quản trị toàn cầu hoặc thông tin thanh toán.</span><span class="sxs-lookup"><span data-stu-id="1f5cc-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="1f5cc-106">Nếu bạn không có TLS 1,2, bạn có thể nhận được lỗi sau đây khi tìm cách nhận hoặc cập nhật chính sách:</span><span class="sxs-lookup"><span data-stu-id="1f5cc-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="1f5cc-107">*Thông báo ErrorMessage-kết nối cơ sở đã được đóng: một lỗi không mong muốn xảy ra khi gửi*.</span><span class="sxs-lookup"><span data-stu-id="1f5cc-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



