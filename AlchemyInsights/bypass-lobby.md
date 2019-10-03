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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376909"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="e6724-102">Kiểm soát cài đặt sảnh và mức độ tham gia</span><span class="sxs-lookup"><span data-stu-id="e6724-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="e6724-103">Các thiết lập kiểm soát mà người tham gia cuộc họp chờ đợi trong hành lang trước khi chúng được nhận vào cuộc họp và mức độ tham gia được cho phép trong một cuộc họp.</span><span class="sxs-lookup"><span data-stu-id="e6724-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e6724-104">Bạn có thể sử dụng PowerShell để cập nhật cài đặt chính sách cuộc họp chưa được triển khai (có nhãn "đến sớm") trong Trung tâm quản trị teams.</span><span class="sxs-lookup"><span data-stu-id="e6724-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="e6724-105">Xem bên dưới để biết lệnh ghép ngắn PowerShell ví dụ cho phép tất cả người dùng bỏ qua hành lang.</span><span class="sxs-lookup"><span data-stu-id="e6724-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="e6724-106">[Tự động thừa nhận người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là chính sách cho mỗi tổ chức điều khiển xem người tham gia cuộc họp trực tiếp hay đợi ở hành lang cho đến khi họ được người dùng xác thực nhận.</span><span class="sxs-lookup"><span data-stu-id="e6724-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e6724-107">[Cho phép người vô danh để bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là chính sách cho một tổ chức điều khiển xem người vô danh, bao gồm người dùng B2B và liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng xác thực từ tổ chức tham dự.</span><span class="sxs-lookup"><span data-stu-id="e6724-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e6724-108">[Cho phép người dùng quay số để bỏ qua hành lang](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức điều khiển xem những người quay số bằng điện thoại có tham gia cuộc họp trực tiếp hay chờ đợi trong hành lang bất kể cài đặt **tự động thừa nhận người** .</span><span class="sxs-lookup"><span data-stu-id="e6724-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e6724-109">[Cho phép người tổ chức ghi đè cài đặt tiền sảnh](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức kiểm soát xem tổ chức cuộc họp có thể ghi đè cài đặt tiền sảnh mà một quản trị viên đặt **tự động thừa** nhận và **cho phép quay số trong người dùng bỏ qua hành lang** khi họ lên lịch cuộc họp mới.</span><span class="sxs-lookup"><span data-stu-id="e6724-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e6724-110">**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) để biết tổng quan đầy đủ về chính sách cuộc họp của Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e6724-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="e6724-111">**Ví dụ về PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e6724-111">**PowerShell example**</span></span>

<span data-ttu-id="e6724-112">Nếu bạn muốn cho phép tất cả mọi người, bao gồm cả người dùng bên ngoài hoặc ẩn danh, để bỏ qua hành lang, bạn cũng có thể sử dụng PowerShell để thực hiện nhiệm vụ này.</span><span class="sxs-lookup"><span data-stu-id="e6724-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="e6724-113">Dưới đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="e6724-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="e6724-114">(Hãy chắc chắn để đánh giá các tài liệu trên trước khi thực hiện những thay đổi này để hiểu chính xác những gì này cho phép.)</span><span class="sxs-lookup"><span data-stu-id="e6724-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="e6724-115">Thiết lập CsTeamsMeetingPolicy-danh tính toàn cầu-AutoAdmittedUsers "tất cả mọi người"-Allowusnuserstobypasslobby $True</span><span class="sxs-lookup"><span data-stu-id="e6724-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="e6724-116">Để biết thêm thông tin, xem [thiết lập CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="e6724-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
