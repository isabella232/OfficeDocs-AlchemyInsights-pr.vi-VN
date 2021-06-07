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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798666"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="feaa9-102">Quản lý đăng ký hội thảo web</span><span class="sxs-lookup"><span data-stu-id="feaa9-102">Manage webinar registration</span></span>

<span data-ttu-id="feaa9-103">Bạn quản lý những người có thể đăng ký Teams Webinars bằng cách sử Teams lệnh Powershell mới.</span><span class="sxs-lookup"><span data-stu-id="feaa9-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="feaa9-104">Để cài Teams Powershell, hãy [xem Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="feaa9-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="feaa9-105">Theo mặc định, *WhoCanRegister* được bật và đặt là Mọi **người**.</span><span class="sxs-lookup"><span data-stu-id="feaa9-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="feaa9-106">Nếu bạn không thấy tùy chọn cho phép đăng ký cho Mọi người trong thư mời họp, hãy chạy lại cài đặt *WhoCanRegister* to Everyone và chờ 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="feaa9-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="feaa9-107">Để chạy lại *WhoCanRegister*, hãy sử dụng lệnh Powershell:</span><span class="sxs-lookup"><span data-stu-id="feaa9-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="feaa9-108">**Lưu ý:** Nếu tham gia ẩn danh được tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web.</span><span class="sxs-lookup"><span data-stu-id="feaa9-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="feaa9-109">Để tìm hiểu thêm và bật thiết đặt này, hãy [xem Quản lý thiết đặt cuộc họp Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="feaa9-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="feaa9-110">Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**</span><span class="sxs-lookup"><span data-stu-id="feaa9-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="feaa9-111">Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="feaa9-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="feaa9-112">Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="feaa9-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
