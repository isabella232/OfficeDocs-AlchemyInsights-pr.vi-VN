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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768462"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="c8424-102">Kiểm soát cài đặt sảnh và mức độ tham gia</span><span class="sxs-lookup"><span data-stu-id="c8424-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="c8424-103">Nếu bạn muốn cho phép mọi người, bao gồm cả người dùng quay số, bên ngoài và ẩn danh để bỏ qua hành lang trong Microsoft teams, bạn có thể sử dụng PowerShell để thực hiện.</span><span class="sxs-lookup"><span data-stu-id="c8424-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="c8424-104">Dưới đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="c8424-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="c8424-105">Lệnh này hiện yêu cầu sử dụng Skype dành cho mô-đun PowerShell kinh doanh.</span><span class="sxs-lookup"><span data-stu-id="c8424-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="c8424-106">Để có được thiết lập để sử dụng lệnh này, hãy kiểm tra [chính sách quản lý qua PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="c8424-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="c8424-107">Bạn có thể thiết lập chính sách mới mà sau đó bạn sẽ cần áp dụng cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="c8424-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="c8424-108">Nếu bạn sửa đổi chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="c8424-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="c8424-109">Đối với bất kỳ thay đổi chính sách nào, bạn cần phải chờ ít nhất 4 giờ và tối đa 24 giờ để các chính sách có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="c8424-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="c8424-110">Hãy chắc chắn để đánh giá các tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những gì này cho phép.</span><span class="sxs-lookup"><span data-stu-id="c8424-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="c8424-111">Hiểu các kiểm soát chính sách của teams họp tại sảnh</span><span class="sxs-lookup"><span data-stu-id="c8424-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="c8424-112">[Tự động thừa nhận người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là chính sách cho mỗi tổ chức điều khiển xem người tham gia cuộc họp trực tiếp hay đợi ở hành lang cho đến khi họ được người dùng xác thực nhận.</span><span class="sxs-lookup"><span data-stu-id="c8424-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c8424-113">[Cho phép người vô danh để bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là chính sách cho một tổ chức điều khiển xem người vô danh, bao gồm người dùng B2B và liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng xác thực từ tổ chức tham dự.</span><span class="sxs-lookup"><span data-stu-id="c8424-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c8424-114">[Cho phép người dùng quay số để bỏ qua hành lang](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức điều khiển xem những người quay số bằng điện thoại có tham gia cuộc họp trực tiếp hay chờ đợi trong hành lang bất kể cài đặt **tự động thừa nhận người** .</span><span class="sxs-lookup"><span data-stu-id="c8424-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c8424-115">[Cho phép người tổ chức ghi đè cài đặt tiền sảnh](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức kiểm soát xem tổ chức cuộc họp có thể ghi đè cài đặt tiền sảnh mà một quản trị viên đặt **tự động thừa** nhận và **cho phép quay số trong người dùng bỏ qua hành lang** khi họ lên lịch cuộc họp mới.</span><span class="sxs-lookup"><span data-stu-id="c8424-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c8424-116">**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) để biết tổng quan đầy đủ về chính sách cuộc họp của Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="c8424-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
