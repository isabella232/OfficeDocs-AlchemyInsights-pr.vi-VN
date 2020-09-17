---
title: Thiết đặt chính sách cuộc họp
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794356"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Quản lý chính sách cuộc họp trong nhóm Microsoft

**Lưu ý: có thể mất đến 24 giờ để thay đổi chính sách có hiệu lực đối với người dùng.** Có thể bạn không thể thực hiện thay đổi đối với các chính sách mới được tạo ngay lập tức; Hãy chờ 4 giờ và cố gắng sửa đổi lại chính sách mới được tạo.

Các chính sách cuộc họp được dùng để điều khiển các tính năng sẵn dùng cho những người dự cuộc họp cho các cuộc họp được lên lịch bởi người dùng trong tổ chức của bạn. Một số tính năng của chính sách cuộc họp có thể không được thực hiện trong Trung tâm quản trị nhóm nào đó (đây là các tính năng có nhãn "Coming Soon" trong tài liệu). Trong trường hợp này, hoặc nếu bạn nhận được lỗi như "chúng tôi không thể cập nhật chính sách ngay bây giờ nhưng thử lại sau" trong Trung tâm quản trị nhóm Microsoft, chúng tôi khuyên bạn nên sử dụng PowerShell để tạo hoặc sửa đổi chính sách cuộc họp nhóm. 

Để biết thêm thông tin về chính sách cuộc họp, hãy xem các tài nguyên sau đây:

- Để tìm hiểu về việc tạo chính sách, thực hiện thay đổi và gán người dùng vào chính sách, hãy xem [quản lý chính sách cuộc họp trong nhóm](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Để thực hiện thay đổi chính sách bằng lệnh ghép ngắn PowerShell, hãy xem [tổng quan về các nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Bạn cần sử dụng [mô-đun của Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) cho các chính sách cuộc họp nhóm. 
    - Xem lại [tài liệu ngắn lệnh ghép ngắn *-csteamsmeetingđể](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) biết thêm thông tin.

