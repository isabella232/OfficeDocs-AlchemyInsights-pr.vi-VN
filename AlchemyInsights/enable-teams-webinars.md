---
title: Bật Hội Teams Web
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794034"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="9923a-102">Bật Hội Teams Web</span><span class="sxs-lookup"><span data-stu-id="9923a-102">Enable Teams Webinars</span></span>

<span data-ttu-id="9923a-103">Hội thảo trên web được bật theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="9923a-103">Webinars are enabled by default.</span></span> <span data-ttu-id="9923a-104">Bạn có thể quản lý những người có thể lên lịch và đăng ký Teams Webinars bằng cách Teams lệnh PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9923a-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="9923a-105">Tất cả người dùng có thể tạo cuộc họp cũng có thể tạo cuộc họp hội thảo web.</span><span class="sxs-lookup"><span data-stu-id="9923a-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="9923a-106">Nếu bạn muốn quản lý những người có thể lên lịch Teams Webinars, hãy sử *dụng AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="9923a-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="9923a-107">Theo mặc định, *WhoCanRegister* được bật và đặt là Mọi **người**.</span><span class="sxs-lookup"><span data-stu-id="9923a-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="9923a-108">Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**</span><span class="sxs-lookup"><span data-stu-id="9923a-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="9923a-109">Để thay đổi các thiết đặt này, bạn [phải cài Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="9923a-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="9923a-110">Ngoài ra, Chính sách Cuộc họp được thực thi Teams Webinars.</span><span class="sxs-lookup"><span data-stu-id="9923a-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="9923a-111">Ví dụ: nếu kết nối ẩn danh bị tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web.</span><span class="sxs-lookup"><span data-stu-id="9923a-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="9923a-112">Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="9923a-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="9923a-113">Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="9923a-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>