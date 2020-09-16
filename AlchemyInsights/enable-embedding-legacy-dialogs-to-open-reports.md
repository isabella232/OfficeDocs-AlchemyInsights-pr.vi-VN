---
title: Bật các hộp thoại kế thừa nhúng để mở báo cáo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806457"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="a3a6d-102">Bật các hộp thoại kế thừa nhúng để mở báo cáo</span><span class="sxs-lookup"><span data-stu-id="a3a6d-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="a3a6d-103">**Chứng**</span><span class="sxs-lookup"><span data-stu-id="a3a6d-103">**Symptom**</span></span>

<span data-ttu-id="a3a6d-104">Người dùng không thể mở báo cáo.</span><span class="sxs-lookup"><span data-stu-id="a3a6d-104">Users are unable to open reports.</span></span> <span data-ttu-id="a3a6d-105">"Có điều gì đó không ổn.</span><span class="sxs-lookup"><span data-stu-id="a3a6d-105">"Something has gone wrong.</span></span> <span data-ttu-id="a3a6d-106">Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "</span><span class="sxs-lookup"><span data-stu-id="a3a6d-106">Check technical details for more details."</span></span>

<span data-ttu-id="a3a6d-107">**Bởi**</span><span class="sxs-lookup"><span data-stu-id="a3a6d-107">**Cause**</span></span>

<span data-ttu-id="a3a6d-108">Báo cáo không tải trong UCI với lỗi, "bộ định dạng biểu mẫu là NULL hoặc không được xác định."</span><span class="sxs-lookup"><span data-stu-id="a3a6d-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="a3a6d-109">Các báo cáo trong UCI vẫn yêu cầu các hộp thoại kế thừa, vì vậy hệ thống của khách hàng cần *phải có được* kích hoạt phân cấp bộ chọn.</span><span class="sxs-lookup"><span data-stu-id="a3a6d-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="a3a6d-110">**Nghiệm**</span><span class="sxs-lookup"><span data-stu-id="a3a6d-110">**Solution**</span></span>

1. <span data-ttu-id="a3a6d-111">Đi đến **thiết đặt >quản trị > thiết đặt hệ thống > tab chung**.</span><span class="sxs-lookup"><span data-stu-id="a3a6d-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="a3a6d-112">Đặt "bật nhúng hộp thoại kế thừa nhất định trong máy khách trình duyệt giao diện hợp nhất" thành **có**.</span><span class="sxs-lookup"><span data-stu-id="a3a6d-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
