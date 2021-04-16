---
title: Bật các hộp thoại kế thừa nhúng để mở báo cáo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814286"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="e6914-102">Bật các hộp thoại kế thừa nhúng để mở báo cáo</span><span class="sxs-lookup"><span data-stu-id="e6914-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="e6914-103">**Chứng**</span><span class="sxs-lookup"><span data-stu-id="e6914-103">**Symptom**</span></span>

<span data-ttu-id="e6914-104">Người dùng không thể mở báo cáo.</span><span class="sxs-lookup"><span data-stu-id="e6914-104">Users are unable to open reports.</span></span> <span data-ttu-id="e6914-105">"Có điều gì đó không ổn.</span><span class="sxs-lookup"><span data-stu-id="e6914-105">"Something has gone wrong.</span></span> <span data-ttu-id="e6914-106">Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "</span><span class="sxs-lookup"><span data-stu-id="e6914-106">Check technical details for more details."</span></span>

<span data-ttu-id="e6914-107">**Bởi**</span><span class="sxs-lookup"><span data-stu-id="e6914-107">**Cause**</span></span>

<span data-ttu-id="e6914-108">Báo cáo không tải trong UCI với lỗi, "bộ định dạng biểu mẫu là NULL hoặc không được xác định."</span><span class="sxs-lookup"><span data-stu-id="e6914-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="e6914-109">Các báo cáo trong UCI vẫn yêu cầu các hộp thoại kế thừa, vì vậy hệ thống của khách hàng cần *phải có được* kích hoạt phân cấp bộ chọn.</span><span class="sxs-lookup"><span data-stu-id="e6914-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="e6914-110">**Nghiệm**</span><span class="sxs-lookup"><span data-stu-id="e6914-110">**Solution**</span></span>

1. <span data-ttu-id="e6914-111">Đi đến **thiết đặt >quản trị > thiết đặt hệ thống > tab chung**.</span><span class="sxs-lookup"><span data-stu-id="e6914-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="e6914-112">Đặt "bật nhúng hộp thoại kế thừa nhất định trong máy khách trình duyệt giao diện hợp nhất" thành **có**.</span><span class="sxs-lookup"><span data-stu-id="e6914-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
