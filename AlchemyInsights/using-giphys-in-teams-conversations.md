---
title: Sử dụng Giphys trong các cuộc hội thoại Nhóm
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982572"
---
# <a name="using-giphys-in-teams-conversations"></a>Sử dụng Giphys trong các cuộc hội thoại Nhóm

Truy nhập giphys trong nhóm trò chuyện được bật theo mặc định. Với tư cách là người quản trị, bạn có thể kiểm soát nếu Giphys sẵn có cho người dùng bằng [cách đặt chính sách gửi tin nhắn](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) và đảm bảo rằng **việc sử dụng giphys trong các cuộc hội thoại** đang **bật**.

Nếu GIFs không hoạt động như dự kiến trong các cuộc hội thoại nhóm, hãy xác nhận:

[Chính sách nhắn tin](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) cần để cho phép Giphys. Để xác nhận bằng cách sử dụng lệnh ghép ngắn PowerShell:

- Xác nhận rằng bạn có thể [quản lý các nhóm bằng PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Chạy lệnh PowerShell [Get-Cisteamsmessagingpolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) và xác minh rằng **allowgiphy** được đặt là **True**.
- Nếu **Allowgiphy** được đặt là **false** , hãy chạy lệnh PowerShell sau đây là lệnh [-Xsteamsmessagingpolicy-Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Những trải nghiệm kết nối tùy chọn](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) cần được kích hoạt để cho phép truy nhập vào URL của giphy.

> [!NOTE]
> Nếu bạn có nhiều chính sách nhắn tin theo nhóm được cấu hình cho đối tượng thuê của mình, bạn có thể xác định danh tính của chính sách được gán cho người dùng bị ảnh hưởng bằng lệnh PowerShell [Get-Xsonlineuser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Chọn TeamsMessagingPolicy.
