---
title: Thiết đặt chính sách cuộc họp
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
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925187"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Quản lý chính sách cuộc họp trong Microsoft Teams

**Lưu ý: Có thể mất tới 24 giờ để thay đổi chính sách có hiệu lực đối với người dùng.** Bạn có thể không thực hiện được thay đổi đối với các chính sách mới được tạo ngay lập tức; hãy chờ 4 giờ và tìm cách sửa đổi lại chính sách mới được tạo.

Chính sách cuộc họp được dùng để kiểm soát các tính năng sẵn dùng cho những người dự cuộc họp đối với các cuộc họp do người dùng trong tổ chức của bạn lên lịch. Một số tính năng của chính sách cuộc họp có thể chưa được thực hiện trong trung tâm quản trị Teams (những tính năng này được gắn nhãn "sắp ra mắt" trong tài liệu). Trong trường hợp này hoặc nếu bạn đang gặp lỗi như "Chúng tôi không thể cập nhật chính sách ngay bây giờ nhưng hãy thử lại sau" trong trung tâm quản trị Microsoft Teams, chúng tôi khuyên bạn nên sử dụng PowerShell để tạo hoặc sửa đổi chính sách cuộc họp Teams. 

Để biết thêm thông tin về chính sách cuộc họp, hãy xem các tài nguyên sau đây:

- Để tìm hiểu về việc tạo chính sách, thực hiện thay đổi và gán người dùng vào chính sách, hãy xem Quản lý chính sách [cuộc họp Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Để thực hiện thay đổi chính sách bằng lệnh ghép ngắn PowerShell, [hãy xem Teams quan về PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Bạn cần sử dụng [mô-đun Skype for Business PowerShell cho chính](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) sách Teams họp mới. 
    - Xem lại [hướng dẫn sử dụng các lệnh ghép ngắn *-CsTeamsMeetingPolicy để](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) biết thêm thông tin.

