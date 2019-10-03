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
# <a name="control-lobby-settings-and-level-of-participation"></a>Kiểm soát cài đặt sảnh và mức độ tham gia

Các thiết lập kiểm soát mà người tham gia cuộc họp chờ đợi trong hành lang trước khi chúng được nhận vào cuộc họp và mức độ tham gia được cho phép trong một cuộc họp. Bạn có thể sử dụng PowerShell để cập nhật cài đặt chính sách cuộc họp chưa được triển khai (có nhãn "đến sớm") trong Trung tâm quản trị teams.  Xem bên dưới để biết lệnh ghép ngắn PowerShell ví dụ cho phép tất cả người dùng bỏ qua hành lang.  

- [Tự động thừa nhận người](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) là chính sách cho mỗi tổ chức điều khiển xem người tham gia cuộc họp trực tiếp hay đợi ở hành lang cho đến khi họ được người dùng xác thực nhận.

- [Cho phép người vô danh để bắt đầu cuộc họp](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) là chính sách cho một tổ chức điều khiển xem người vô danh, bao gồm người dùng B2B và liên kết, có thể tham gia cuộc họp của người dùng mà không có người dùng xác thực từ tổ chức tham dự.

- [Cho phép người dùng quay số để bỏ qua hành lang](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức điều khiển xem những người quay số bằng điện thoại có tham gia cuộc họp trực tiếp hay chờ đợi trong hành lang bất kể cài đặt **tự động thừa nhận người** .

- [Cho phép người tổ chức ghi đè cài đặt tiền sảnh](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**sắp ra mắt**) là chính sách cho mỗi tổ chức kiểm soát xem tổ chức cuộc họp có thể ghi đè cài đặt tiền sảnh mà một quản trị viên đặt **tự động thừa** nhận và **cho phép quay số trong người dùng bỏ qua hành lang** khi họ lên lịch cuộc họp mới.

**Lưu ý:** Đọc [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) để biết tổng quan đầy đủ về chính sách cuộc họp của Microsoft teams. 


**Ví dụ về PowerShell**

Nếu bạn muốn cho phép tất cả mọi người, bao gồm cả người dùng bên ngoài hoặc ẩn danh, để bỏ qua hành lang, bạn cũng có thể sử dụng PowerShell để thực hiện nhiệm vụ này.  Dưới đây là ví dụ về sửa đổi chính sách cuộc họp toàn cầu cho tổ chức của bạn.   

(Hãy chắc chắn để đánh giá các tài liệu trên trước khi thực hiện những thay đổi này để hiểu chính xác những gì này cho phép.)

Thiết lập CsTeamsMeetingPolicy-danh tính toàn cầu-AutoAdmittedUsers "tất cả mọi người"-Allowusnuserstobypasslobby $True

Để biết thêm thông tin, xem [thiết lập CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
