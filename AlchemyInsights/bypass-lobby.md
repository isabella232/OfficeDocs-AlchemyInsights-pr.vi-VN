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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kiểm soát các thiết đặt phòng đợi và mức độ tham gia trong nhóm

Nếu bạn muốn cho phép mọi người, bao gồm cả những người dùng quay số vào, bên ngoài và ẩn danh, để **bỏ qua phòng đợi**, hãy dùng PowerShell để thực hiện tác vụ này. Đây là một ví dụ về việc sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Lệnh ghép ngắn này hiện đang yêu cầu sử dụng mô-đun của Skype for Business PowerShell. Để được thiết lập để sử dụng lệnh ghép ngắn này, hãy xem phần [quản lý chính sách qua PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Sau khi bạn đã thiết lập chính sách, bạn cần áp dụng nó cho người dùng; hoặc nếu bạn đã sửa đổi chính sách toàn cầu, nó sẽ tự động áp dụng cho người dùng. Đối với bất kỳ thay đổi chính sách nào, bạn cần chờ ít nhất **4 giờ tối đa 24 giờ** để các chính sách có hiệu lực. 

Hãy đảm bảo bạn xem lại tài liệu dưới đây trước khi thực hiện những thay đổi này để hiểu chính xác những điều này cho phép.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Tìm hiểu về điều khiển chính sách phòng đợi cuộc họp nhóm

Những thiết đặt này kiểm soát những người dự cuộc họp chờ đợi trong phòng đợi trước khi chúng được nhận vào cuộc họp và mức độ tham gia của họ được phép trong cuộc họp. Bạn có thể sử dụng PowerShell để cập nhật các thiết đặt chính sách cuộc họp chưa được thực hiện (có nhãn "Coming Soon") trong Trung tâm quản trị nhóm. Xem phần dưới đây cho một lệnh ghép ngắn PowerShell ví dụ cho phép tất cả người dùng bỏ qua phòng đợi.

- [Tự động thừa nhận mọi người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là một chính sách cho mỗi người tổ chức điều khiển cho dù mọi người tham gia cuộc họp trực tiếp hoặc chờ trong phòng đợi cho đến khi chúng được người dùng xác thực thừa nhận.

- [Cho phép những người ẩn danh bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là một chính sách cho mỗi người tổ chức điều khiển cho dù những người ẩn danh, bao gồm B2B và người dùng liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng được xác thực từ tổ chức tham dự.

- [Cho phép người dùng quay số vào bỏ qua phòng đợi](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp**ra mắt) là chính sách cho mỗi người tổ chức điều khiển cho dù những người quay số vào bằng điện thoại sẽ tham gia cuộc họp trực tiếp hoặc chờ trong phòng đợi, bất kể thiết đặt **mọi người tự động thừa nhận** .

- [Cho phép người tổ chức ghi đè các thiết đặt](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) phòng chờ (**sắp**ra mắt) là chính sách cho mỗi người tổ chức kiểm soát việc người tổ chức cuộc họp có thể ghi đè lên các thiết đặt phòng đợi mà người quản trị đã đặt **tự động thừa nhận** và **cho phép người dùng quay số** vào khi họ lên lịch một cuộc họp mới.

**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong nhóm](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) để biết tổng quan về chính sách cuộc họp Microsoft nhóm.
