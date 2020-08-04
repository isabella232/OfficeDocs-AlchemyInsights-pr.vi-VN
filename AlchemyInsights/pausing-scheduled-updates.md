---
title: Tạm dừng Cập Nhật theo lịch
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555995"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="352d6-102">Tạm dừng Cập Nhật theo lịch</span><span class="sxs-lookup"><span data-stu-id="352d6-102">Pausing scheduled updates</span></span>

<span data-ttu-id="352d6-103">Khi lệnh tạm dừng được phát hành, thiết bị không xử lý lệnh cho đến lần tiếp theo họ kiểm tra InTune.</span><span class="sxs-lookup"><span data-stu-id="352d6-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="352d6-104">Do đó, các thiết bị của bạn có thể có:</span><span class="sxs-lookup"><span data-stu-id="352d6-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="352d6-105">Cài đặt bản Cập Nhật đã lên lịch trước khi nhận phòng.</span><span class="sxs-lookup"><span data-stu-id="352d6-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="352d6-106">Đã được tắt nguồn khi bạn phát hành lệnh tạm dừng.</span><span class="sxs-lookup"><span data-stu-id="352d6-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="352d6-107">Trong trường hợp này, khi các thiết bị được bật, họ có thể đã tải xuống và cài đặt các bản Cập Nhật đã lên lịch trước khi nhận phòng.</span><span class="sxs-lookup"><span data-stu-id="352d6-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>