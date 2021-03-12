---
title: bản ghi cuộc gọi 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733871"
---
# <a name="11-call-recording"></a><span data-ttu-id="96251-102">bản ghi cuộc gọi 1:1</span><span class="sxs-lookup"><span data-stu-id="96251-102">1:1 call recording</span></span>

<span data-ttu-id="96251-103">Người quản trị cần thực hiện hành động để tiếp tục cho phép người dùng ghi lại cuộc gọi 1:1.</span><span class="sxs-lookup"><span data-stu-id="96251-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="96251-104">Bắt đầu từ ngày 12/04/2018, 2021, chúng tôi sẽ bắt đầu thực thi tùy chọn chính sách gọi nhóm mới trong *Allowcloudrecordingforcalls*.</span><span class="sxs-lookup"><span data-stu-id="96251-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="96251-105">Hiện tại, các chức năng ghi cuộc gọi 1:1 được điều khiển bởi tùy chọn *Allowcloudrecording* trong chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="96251-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="96251-106">Nếu người dùng của bạn được phép ghi lại cuộc họp nhóm, họ cũng có thể ghi lại các cuộc gọi 1:1.</span><span class="sxs-lookup"><span data-stu-id="96251-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="96251-107">Nếu bạn muốn chặn tất cả người dùng ghi lại cuộc gọi 1:1, bạn không cần thực hiện bất kỳ hành động nào.</span><span class="sxs-lookup"><span data-stu-id="96251-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="96251-108">Tùy chọn chính sách gọi cho *Allowcloudrecordingforcalls* sẽ được $false theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="96251-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="96251-109">Thay đổi này được tài liệu trong bài đăng của Trung tâm thông báo sau: [(Cập Nhật) 1:1 gọi giới thiệu chính sách ghi âm](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) để đặt tùy chọn chính sách gọi nhóm, bạn phải sử dụng [nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="96251-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="96251-110">**Để bật ghi cuộc gọi trong 1:1 cuộc gọi:** Set-CsTeamsCallingPolicy-căn cước cho các cuộc gọi toàn cầu-Allowcloudrecording$True</span><span class="sxs-lookup"><span data-stu-id="96251-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="96251-111">**Để tắt tính năng ghi cuộc gọi trong 1:1 cuộc gọi:** Set-CsTeamsCallingPolicy-căn cước các cuộc gọi toàn cầu-allowcloudtheo $false</span><span class="sxs-lookup"><span data-stu-id="96251-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

