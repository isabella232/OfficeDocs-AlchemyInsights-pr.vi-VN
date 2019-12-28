---
title: Hành lang Bypass
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889104"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="e7b61-102">Cài đặt kiểm soát hành lang và mức độ tham gia của teams</span><span class="sxs-lookup"><span data-stu-id="e7b61-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="e7b61-103">Nếu bạn muốn cho phép tất cả mọi người, bao gồm cả người dùng quay số, bên ngoài và ẩn danh, để **bỏ qua hành lang, hãy**sử dụng PowerShell để thực hiện tác vụ này.</span><span class="sxs-lookup"><span data-stu-id="e7b61-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="e7b61-104">Dưới đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="e7b61-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="e7b61-105">Lệnh này hiện yêu cầu sử dụng Skype dành cho mô-đun PowerShell kinh doanh.</span><span class="sxs-lookup"><span data-stu-id="e7b61-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="e7b61-106">Để được thiết lập để sử dụng lệnh này, hãy kiểm tra [chính sách quản lý qua PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="e7b61-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="e7b61-107">Sau khi thiết lập chính sách, bạn cần phải áp dụng cho người dùng; hoặc, nếu bạn sửa đổi chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="e7b61-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="e7b61-108">Đối với bất kỳ thay đổi chính sách, bạn cần phải chờ ít nhất **4 giờ tối đa 24 giờ** để các chính sách có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="e7b61-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="e7b61-109">Hãy chắc chắn để đánh giá các tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những gì này cho phép.</span><span class="sxs-lookup"><span data-stu-id="e7b61-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="e7b61-110">Hiểu các kiểm soát chính sách của teams họp tại sảnh</span><span class="sxs-lookup"><span data-stu-id="e7b61-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="e7b61-111">Các thiết lập kiểm soát mà người tham gia cuộc họp chờ đợi trong hành lang trước khi chúng được nhận vào cuộc họp và mức độ tham gia được cho phép trong một cuộc họp.</span><span class="sxs-lookup"><span data-stu-id="e7b61-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e7b61-112">Bạn có thể sử dụng PowerShell để cập nhật cài đặt chính sách cuộc họp chưa được thực hiện (có nhãn "đến sớm") trong Trung tâm quản trị teams.</span><span class="sxs-lookup"><span data-stu-id="e7b61-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="e7b61-113">Xem bên dưới để biết lệnh ghép ngắn PowerShell ví dụ cho phép tất cả người dùng bỏ qua hành lang.</span><span class="sxs-lookup"><span data-stu-id="e7b61-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="e7b61-114">[Tự động thừa nhận người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là chính sách cho mỗi tổ chức điều khiển xem người tham gia cuộc họp trực tiếp hay đợi ở hành lang cho đến khi họ được người dùng xác thực nhận.</span><span class="sxs-lookup"><span data-stu-id="e7b61-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e7b61-115">[Cho phép người vô danh để bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là chính sách cho một tổ chức điều khiển xem người vô danh, bao gồm người dùng B2B và liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng xác thực từ tổ chức tham dự.</span><span class="sxs-lookup"><span data-stu-id="e7b61-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e7b61-116">[Cho phép người dùng quay số để bỏ qua hành lang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức điều khiển xem những người quay số bằng điện thoại có tham gia cuộc họp trực tiếp hay chờ đợi trong hành lang bất kể cài đặt **tự động thừa nhận người** .</span><span class="sxs-lookup"><span data-stu-id="e7b61-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e7b61-117">[Cho phép người tổ chức ghi đè cài đặt tiền sảnh](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**sắp ra mắt**) là một tổ chức chính sách điều khiển xem tổ chức cuộc họp có thể ghi đè các thiết đặt tiền sảnh mà một quản trị viên đặt **tự động thừa** nhận và **cho phép người dùng quay số để vượt qua hành lang** khi họ lên lịch một cuộc họp mới.</span><span class="sxs-lookup"><span data-stu-id="e7b61-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e7b61-118">**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) để biết tổng quan đầy đủ về chính sách cuộc họp của Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e7b61-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
