---
title: Di chuyển thư mục công cộng không thành công tại 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803929"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="9f47e-102">Di chuyển thư mục công cộng không thành công tại 95%</span><span class="sxs-lookup"><span data-stu-id="9f47e-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="9f47e-103">Bạn có thể đã bắt đầu hoàn thành một lô di chuyển và trạng thái của lô di chuyển vẫn tiếp **tục hiển thị** được đồng bộ trong một thời gian rất dài.</span><span class="sxs-lookup"><span data-stu-id="9f47e-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="9f47e-104">Đây là hành vi dự kiến.</span><span class="sxs-lookup"><span data-stu-id="9f47e-104">This is expected behavior.</span></span>

<span data-ttu-id="9f47e-105">Nó phổ **biến cho trạng** Thái của lô di chuyển vẫn tiếp tục được đồng bộ trong một vài giờ trước khi chuyển đổi để **hoàn thành**.</span><span class="sxs-lookup"><span data-stu-id="9f47e-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="9f47e-106">Để di chuyển liên quan đến một số lượng lớn các hộp thư đích, thông thường là bạn sẽ thấy trạng thái vẫn giữ nguyên trong trạng thái đồng bộ trong hơn 24 giờ, không cung cấp các yêu cầu di chuyển thư mục công cộng nằm bên dưới.</span><span class="sxs-lookup"><span data-stu-id="9f47e-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="9f47e-107">Vui lòng cho phép 24-48 giờ cho lô di chuyển để hoàn thành nhiệm vụ.</span><span class="sxs-lookup"><span data-stu-id="9f47e-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="9f47e-108">Đối với việc di chuyển thư mục công cộng không tại 95%, với lỗi FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="9f47e-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="9f47e-109">Tải xuống và chạy tập lệnh [thư mục Validatemailenabledtại](https://aka.ms/ValidateMEPF) máy chủ Exchange tại cơ sở của bạn.</span><span class="sxs-lookup"><span data-stu-id="9f47e-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="9f47e-110">Thực hiện các hành động khắc phục được đề xuất bởi tập lệnh.</span><span class="sxs-lookup"><span data-stu-id="9f47e-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="9f47e-111">Chạy thư mục đồng bộ (dành cho Exchange 2010) hoặc thư mục đồng bộ hóa (dành cho Exchange 2013 trở lên).</span><span class="sxs-lookup"><span data-stu-id="9f47e-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="9f47e-112">Tiếp tục di chuyển thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="9f47e-112">Resume public folder migration.</span></span>
