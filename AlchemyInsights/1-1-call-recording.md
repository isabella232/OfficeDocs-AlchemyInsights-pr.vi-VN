---
title: Ghi âm cuộc gọi 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696980"
---
# <a name="11-call-recording"></a><span data-ttu-id="43747-102">Ghi âm cuộc gọi 1:1</span><span class="sxs-lookup"><span data-stu-id="43747-102">1:1 call recording</span></span>

<span data-ttu-id="43747-103">Nếu nút **Bắt đầu Ghi** bị mờ trong cuộc gọi 1:1, bạn cần thay đổi cài đặt chính sách cho người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="43747-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="43747-104">Bắt đầu từ ngày 31 tháng 5 năm 2021, chúng tôi sẽ bắt đầu thực thi một Chính sách Gọi điện Teams *mới AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="43747-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="43747-105">Trước thay đổi này, việc ghi lại cuộc gọi 1:1 được kiểm soát bởi Chính sách *Cho* phép Ghi Teams họp.</span><span class="sxs-lookup"><span data-stu-id="43747-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="43747-106">Thay đổi này được ghi trong bài đăng trong Trung tâm Thông báo: [(Đã cập nhật) 1:1 Giới thiệu chính sách ghi âm cuộc gọi](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="43747-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="43747-107">*AllowCloudRecordingForCalls*   tùy chọn chính sách cuộc gọi được đặt **thành $False** định.</span><span class="sxs-lookup"><span data-stu-id="43747-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="43747-108">Nếu bạn muốn chặn tất cả người dùng khỏi bản ghi cuộc gọi 1:1, bạn không cần thực hiện bất kỳ hành động nào.</span><span class="sxs-lookup"><span data-stu-id="43747-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="43747-109">Để bật ghi âm cuộc gọi cho tất cả người dùng trong cuộc gọi 1:1, hãy sử Teams PowerShell để chạy lệnh ghép ngắn sau:</span><span class="sxs-lookup"><span data-stu-id="43747-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="43747-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="43747-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="43747-111">Ngoài ra, bạn có thể tạo một chính sách mới và đặt **-AllowCloudRecordingForCalls** **thành $true** và gán chính sách đó cho người dùng của bạn.</span><span class="sxs-lookup"><span data-stu-id="43747-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="43747-112">Để biết thêm thông tin, hãy xem Mục Điều khiển Chính sách Ghi Âm Cuộc gọi [1:1 (Gần như!) Tại đây](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="43747-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
