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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104330"
---
# <a name="using-giphys-in-teams-conversations"></a>Sử dụng Giphy trong Teams thoại

Quyền truy nhập Giphys Teams trò chuyện được bật theo mặc định. Là người quản trị, bạn có thể kiểm [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) soát xem Giphy có sẵn dùng cho người dùng không bằng cách thiết đặt chính sách nhắn tin và đảm bảo rằng Sử dụng **Giphy trong** cuộc hội thoại là **Bật**.

Nếu GIF không hoạt động như mong đợi trong cuộc hội thoại Teams, hãy xác nhận:

Chính [sách nhắn tin](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) cần phải cho phép Giphys. Để xác minh bằng cách sử dụng lệnh ghép ngắn PowerShell:

- Xác minh rằng bạn [có thể Quản Teams với PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Chạy lệnh PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) và xác minh rằng **AllowGiphy** được đặt thành **TRUE.**
- Nếu **AllowGiphy** được đặt thành **FALSE**, hãy chạy lệnh PowerShell [set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.

> [!NOTE]
> Nếu bạn có nhiều chính sách Teams Messaging được cấu hình cho đối tượng thuê của mình, bạn có thể xác định danh tính của chính sách được gán cho người dùng bị ảnh hưởng bằng lệnh [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Chọn TeamsMessagingPolicy.
