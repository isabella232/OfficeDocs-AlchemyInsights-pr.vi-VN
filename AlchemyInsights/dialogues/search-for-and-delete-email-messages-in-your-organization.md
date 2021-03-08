---
title: Tìm kiếm và xóa thông điệp email trong tổ chức của bạn
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527276"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="22e1d-102">Tìm kiếm và xóa thông điệp email trong tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="22e1d-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="22e1d-103">Làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="22e1d-103">Follow these steps:</span></span>

1. <span data-ttu-id="22e1d-104">Nếu bạn không phải là người quản trị toàn cầu, để tìm kiếm thư tài khoản của bạn phải được thêm vào **nhóm vai trò trình quản lý Ekhám phá** hoặc **vai trò quản lý tìm kiếm tuân thủ**.</span><span class="sxs-lookup"><span data-stu-id="22e1d-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="22e1d-105">Để xóa thư, bạn sẽ cần phải tham gia vào **nhóm vai trò quản lý tổ chức** hoặc **vai trò tìm kiếm và dọn sạch quản lý**.</span><span class="sxs-lookup"><span data-stu-id="22e1d-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="22e1d-106">Quyền đối với các vai trò này được gán trong [Trung tâm tuân thủ & bảo mật.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="22e1d-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="22e1d-107">[Tạo một tìm kiếm nội dung](https://docs.microsoft.com/office365/securitycompliance/content-search) để tìm thư cần xóa.</span><span class="sxs-lookup"><span data-stu-id="22e1d-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="22e1d-108">[Kết nối với Trung tâm bảo mật & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="22e1d-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="22e1d-109">Nếu bạn đang sử dụng MFA, hãy xem các hướng dẫn sau: [kết nối với Trung tâm bảo mật & PowerShell bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="22e1d-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="22e1d-110">Xóa bỏ thư: chạy `New-ComplianceSearchAction` lệnh ghép ngắn để xóa thư.</span><span class="sxs-lookup"><span data-stu-id="22e1d-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="22e1d-111">Thư đã xóa được di chuyển đến thư mục các mục có thể phục hồi của người dùng.</span><span class="sxs-lookup"><span data-stu-id="22e1d-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="22e1d-112">Đối với lệnh ví dụ, hãy xem [bước 3: xóa thư.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="22e1d-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
