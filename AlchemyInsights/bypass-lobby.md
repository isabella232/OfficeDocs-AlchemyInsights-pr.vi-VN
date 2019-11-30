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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626370"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Kiểm soát cài đặt sảnh và mức độ tham gia

Nếu bạn muốn cho phép mọi người, bao gồm cả người dùng quay số, bên ngoài và ẩn danh để bỏ qua hành lang trong Microsoft teams, bạn có thể sử dụng PowerShell để thực hiện. Dưới đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Lệnh này hiện yêu cầu sử dụng Skype dành cho mô-đun PowerShell kinh doanh. Để có được thiết lập để sử dụng lệnh này, hãy kiểm tra [chính sách quản lý qua PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Bạn có thể thiết lập chính sách mới mà sau đó bạn sẽ cần áp dụng cho người dùng. Nếu bạn sửa đổi chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng. Đối với bất kỳ thay đổi chính sách nào, bạn cần phải chờ ít nhất 4 giờ và tối đa 24 giờ để các chính sách có hiệu lực.

Hãy chắc chắn để đánh giá các tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những gì này cho phép.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Hiểu các kiểm soát chính sách của teams họp tại sảnh

- [Tự động thừa nhận người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là chính sách cho mỗi tổ chức điều khiển xem người tham gia cuộc họp trực tiếp hay đợi ở hành lang cho đến khi họ được người dùng xác thực nhận.

- [Cho phép người vô danh để bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là chính sách cho một tổ chức điều khiển xem người vô danh, bao gồm người dùng B2B và liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng xác thực từ tổ chức tham dự.

- [Cho phép người dùng quay số để bỏ qua hành lang](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức điều khiển xem những người quay số bằng điện thoại có tham gia cuộc họp trực tiếp hay chờ đợi trong hành lang bất kể cài đặt **tự động thừa nhận người** .

- [Cho phép người tổ chức ghi đè cài đặt tiền sảnh](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**sắp ra mắt**) là một tổ chức chính sách điều khiển xem tổ chức cuộc họp có thể ghi đè các thiết đặt tiền sảnh mà một quản trị viên đặt **tự động thừa** nhận và **cho phép người dùng quay số để vượt qua hành lang** khi họ lên lịch một cuộc họp mới.

**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) để biết tổng quan đầy đủ về chính sách cuộc họp của Microsoft teams.
