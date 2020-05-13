---
title: Cho phép nhúng hộp thoại kế thừa để mở báo cáo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204681"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="84585-102">Cho phép nhúng hộp thoại kế thừa để mở báo cáo</span><span class="sxs-lookup"><span data-stu-id="84585-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="84585-103">**Triệu chứng**</span><span class="sxs-lookup"><span data-stu-id="84585-103">**Symptom**</span></span>

<span data-ttu-id="84585-104">Người dùng không thể mở báo cáo.</span><span class="sxs-lookup"><span data-stu-id="84585-104">Users are unable to open reports.</span></span> <span data-ttu-id="84585-105">"Cái gì đã đi sai.</span><span class="sxs-lookup"><span data-stu-id="84585-105">"Something has gone wrong.</span></span> <span data-ttu-id="84585-106">Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "</span><span class="sxs-lookup"><span data-stu-id="84585-106">Check technical details for more details."</span></span>

<span data-ttu-id="84585-107">**Gây ra**</span><span class="sxs-lookup"><span data-stu-id="84585-107">**Cause**</span></span>

<span data-ttu-id="84585-108">Báo cáo không tải UCI với lỗi "mô tả mẫu là NULL hoặc không xác định."</span><span class="sxs-lookup"><span data-stu-id="84585-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="84585-109">Báo cáo trong UCI vẫn yêu cầu hộp thoại kế thừa, do đó, Hệ thống của khách hàng cần phải có *allowlegacydialogsembedding* kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="84585-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="84585-110">**Giải pháp**</span><span class="sxs-lookup"><span data-stu-id="84585-110">**Solution**</span></span>

1. <span data-ttu-id="84585-111">Đi tới **cài đặt >quản trị > thiết đặt hệ thống > tab chung**.</span><span class="sxs-lookup"><span data-stu-id="84585-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="84585-112">Đặt "bật nhúng các hộp thoại kế thừa nhất định trong ứng dụng trình duyệt giao diện hợp nhất" thành **có**.</span><span class="sxs-lookup"><span data-stu-id="84585-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
