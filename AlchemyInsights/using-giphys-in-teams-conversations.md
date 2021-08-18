---
title: Sử dụng Giphy trong Teams thoại
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323542"
---
# <a name="using-giphys-in-teams-conversations"></a>Sử dụng Giphy trong Teams thoại

Quyền truy nhập giphys Teams trò chuyện được bật theo mặc định. Là người quản trị, bạn có thể kiểm [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) soát xem Giphy có sẵn dùng cho người dùng không bằng cách thiết đặt chính sách nhắn tin và đảm bảo rằng Sử dụng **Giphy trong** cuộc hội thoại là **Bật**.

Nếu GIF không hoạt động như mong đợi trong cuộc hội thoại Teams, hãy xác nhận:

Chính [sách nhắn tin](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) cần phải cho phép Giphys. Để xác minh bằng cách sử dụng lệnh ghép ngắn PowerShell:

- Xác minh rằng bạn [có thể Quản Teams với PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Chạy lệnh PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) và xác minh rằng **AllowGiphy** được đặt thành **TRUE.**
- Nếu **AllowGiphy** được đặt thành **FALSE**, hãy chạy lệnh PowerShell [set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.

Lưu ý **:** Nếu bạn đã cấu hình nhiều chính sách Nhắn tin Teams cho đối tượng thuê của mình, bạn có thể xác định danh tính của chính sách được gán cho người dùng bị ảnh hưởng bằng lệnh PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Chọn TeamsMessagingPolicy.
