---
title: Bỏ qua phòng đợi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684972"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="da943-102">Kiểm soát các thiết đặt phòng đợi và mức độ tham gia trong nhóm</span><span class="sxs-lookup"><span data-stu-id="da943-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="da943-103">Nếu bạn muốn cho phép mọi người, bao gồm cả những người dùng quay số vào, bên ngoài và ẩn danh, để **bỏ qua phòng đợi**, hãy dùng PowerShell để thực hiện tác vụ này.</span><span class="sxs-lookup"><span data-stu-id="da943-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="da943-104">Đây là một ví dụ về việc sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="da943-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="da943-105">Lệnh ghép ngắn này hiện đang yêu cầu sử dụng mô-đun của Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="da943-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="da943-106">Để được thiết lập để sử dụng lệnh ghép ngắn này, hãy xem phần [quản lý chính sách qua PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="da943-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="da943-107">Sau khi bạn đã thiết lập chính sách, bạn cần áp dụng nó cho người dùng; hoặc nếu bạn đã sửa đổi chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="da943-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="da943-108">Đối với bất kỳ thay đổi chính sách nào, bạn cần chờ ít nhất **4 giờ tối đa 24 giờ** để các chính sách có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="da943-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="da943-109">Hãy đảm bảo bạn xem lại tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những điều này cho phép.</span><span class="sxs-lookup"><span data-stu-id="da943-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="da943-110">Tìm hiểu về điều khiển chính sách phòng đợi cuộc họp nhóm</span><span class="sxs-lookup"><span data-stu-id="da943-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="da943-111">Những thiết đặt này kiểm soát những người dự cuộc họp chờ đợi trong phòng đợi trước khi chúng được nhận vào cuộc họp và mức độ tham gia của họ được phép trong cuộc họp.</span><span class="sxs-lookup"><span data-stu-id="da943-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="da943-112">Bạn có thể sử dụng PowerShell để cập nhật các thiết đặt chính sách cuộc họp chưa được thực hiện (có nhãn "Coming Soon") trong Trung tâm quản trị nhóm.</span><span class="sxs-lookup"><span data-stu-id="da943-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="da943-113">Xem phần dưới đây cho một lệnh ghép ngắn PowerShell ví dụ cho phép tất cả người dùng bỏ qua phòng đợi.</span><span class="sxs-lookup"><span data-stu-id="da943-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="da943-114">[Tự động thừa nhận mọi người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là một chính sách cho mỗi người tổ chức điều khiển cho dù mọi người tham gia cuộc họp trực tiếp hoặc chờ trong phòng đợi cho đến khi chúng được người dùng xác thực thừa nhận.</span><span class="sxs-lookup"><span data-stu-id="da943-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="da943-115">[Cho phép những người ẩn danh bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là một chính sách cho mỗi người tổ chức điều khiển cho dù những người ẩn danh, bao gồm B2B và người dùng liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng được xác thực từ tổ chức tham dự.</span><span class="sxs-lookup"><span data-stu-id="da943-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="da943-116">[Cho phép người dùng quay số vào bỏ qua phòng đợi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp**ra mắt) là chính sách cho mỗi người tổ chức điều khiển cho dù những người quay số vào bằng điện thoại sẽ tham gia cuộc họp trực tiếp hoặc chờ trong phòng đợi, bất kể thiết đặt **mọi người tự động thừa nhận** .</span><span class="sxs-lookup"><span data-stu-id="da943-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="da943-117">[Cho phép người tổ chức ghi đè các thiết đặt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) phòng chờ (**sắp**ra mắt) là chính sách cho mỗi người tổ chức kiểm soát việc người tổ chức cuộc họp có thể ghi đè lên các thiết đặt phòng đợi mà người quản trị đã đặt **tự động thừa nhận** và **cho phép người dùng quay số** vào khi họ lên lịch một cuộc họp mới.</span><span class="sxs-lookup"><span data-stu-id="da943-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="da943-118">**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong nhóm](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) để biết tổng quan về chính sách cuộc họp Microsoft nhóm.</span><span class="sxs-lookup"><span data-stu-id="da943-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
