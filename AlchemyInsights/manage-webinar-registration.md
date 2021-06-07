---
title: Quản lý đăng ký hội thảo web
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794141"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2bbf6-102">Quản lý đăng ký hội thảo web</span><span class="sxs-lookup"><span data-stu-id="2bbf6-102">Manage webinar registration</span></span>

<span data-ttu-id="2bbf6-103">Bạn quản lý những người có thể đăng ký Teams Webinars bằng cách sử Teams lệnh Powershell mới.</span><span class="sxs-lookup"><span data-stu-id="2bbf6-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="2bbf6-104">Để cài Teams Powershell, hãy [xem Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="2bbf6-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="2bbf6-105">Theo mặc định, *WhoCanRegister* được bật và đặt thành **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="2bbf6-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="2bbf6-106">Để cho phép bất kỳ ai, bao gồm người  dùng ẩn danh, đăng ký, bạn phải đặt Chính sách Cuộc họp cho Mọi người bằng cách sử dụng lệnh Powershell:</span><span class="sxs-lookup"><span data-stu-id="2bbf6-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="2bbf6-107">**Lưu ý:** Nếu tham gia ẩn danh được tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web.</span><span class="sxs-lookup"><span data-stu-id="2bbf6-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="2bbf6-108">Để tìm hiểu thêm và bật thiết đặt này, hãy [xem Quản lý thiết đặt cuộc họp Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="2bbf6-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="2bbf6-109">Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**</span><span class="sxs-lookup"><span data-stu-id="2bbf6-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2bbf6-110">Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="2bbf6-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2bbf6-111">Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="2bbf6-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
