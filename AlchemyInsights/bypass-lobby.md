---
title: Phòng đợi bỏ qua
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059618"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kiểm soát thiết đặt phòng đợi và cấp độ tham gia trong Teams

Nếu bạn muốn cho phép tất cả mọi người, bao gồm người dùng Quay số vào, bên ngoài và ẩn danh, bỏ qua phòng **đợi,** hãy sử dụng PowerShell để thực hiện tác vụ này. Đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Lệnh ghép ngắn này hiện yêu cầu sử dụng Skype for Business-đun PowerShell của bạn. Để được thiết lập sử dụng lệnh ghép ngắn này, hãy xem qua [mục Quản lý chính sách qua PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Sau khi đã thiết lập chính sách, bạn cần áp dụng chính sách đó cho người dùng; hoặc, nếu bạn đã sửa đổi Chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng. Đối với bất kỳ thay đổi chính sách nào, bạn cần chờ ít nhất 4 giờ đến **24** giờ để các chính sách có hiệu lực. 

Hãy nhớ xem lại tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những gì điều này cho phép.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Tìm hiểu về Teams chính sách phòng đợi cuộc họp

Những thiết đặt này kiểm soát những người dự cuộc họp nào chờ ở phòng đợi trước khi họ được tiếp nhận vào cuộc họp và mức độ tham gia mà họ được phép trong cuộc họp. Bạn có thể sử dụng PowerShell để cập nhật cài đặt chính sách cuộc họp chưa được thực hiện (có nhãn "sắp ra mắt") trong Trung tâm quản trị Teams chính thức. Hãy xem bên dưới để biết ví dụ về lệnh ghép ngắn PowerShell cho phép tất cả người dùng bỏ qua phòng đợi.

- [Tự động chấp nhận mọi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) người là một chính sách cho mỗi người tổ chức kiểm soát việc mọi người có tham dự cuộc họp trực tiếp hay chờ ở phòng đợi cho đến khi họ được một người dùng xác thực tiếp nhận.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Cho phép người ẩn danh bắt đầu cuộc họp là một chính sách theo người tổ chức kiểm soát việc liệu những người ẩn danh, bao gồm B2B và người dùng được liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng đã xác thực từ tổ chức tham dự hay không.

- Cho phép người dùng quay số vào bỏ qua phòng đợi [(sắp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ra mắt **)** là chính sách từng người tổ chức kiểm soát việc những người quay số vào bằng điện thoại có gia nhập trực tiếp vào cuộc họp hay chờ ở phòng đợi bất kể thiết đặt Tự động tiếp nhận mọi **người.**

- Cho phép người tổ chức ghi đè lên thiết đặt phòng đợi [(](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) sắp ra mắt **)** là chính sách  từng người  tổ chức kiểm soát việc người tổ chức cuộc họp có thể ghi đè lên thiết đặt phòng đợi mà người quản trị đã đặt trong Tự động tiếp nhận mọi người và Cho phép người dùng quay số vào bỏ qua phòng đợi khi họ lên lịch cuộc họp mới hay không.

**Lưu ý:** Hãy đọc [Quản lý chính sách cuộc họp Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) để có cái nhìn tổng quan đầy đủ về các chính Microsoft Teams họp.
