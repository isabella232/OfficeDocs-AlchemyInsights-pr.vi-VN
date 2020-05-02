---
title: Kênh riêng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005460"
---
# <a name="private-channels-in-microsoft-teams"></a>Kênh riêng tư trong Microsoft teams

Các kênh riêng tư là một tính năng mới trong Microsoft teams. Lưu ý rằng các kênh riêng tư không thể chuyển đổi từ các kênh tiêu chuẩn hoặc ngược lại.

Để biết chi tiết về các kênh riêng tư, chẳng hạn như thông tin về [việc tạo kênh riêng và](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [các trang web SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)riêng tư và kênh tư nhân, xem [các kênh riêng tư trong Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Lưu ý:** Vì cấu hình để lưu giữ các thư riêng tư không được hỗ trợ, người thuê với chính sách lưu giữ cho phép sẽ không có kênh riêng được kích hoạt theo mặc định. Bạn có thể bật các kênh riêng tư trong Trung tâm quản trị teams. Ngoài ra, lưu ý rằng mặc dù không hỗ trợ lưu trữ các tin nhắn kênh riêng tư, việc lưu giữ các tệp được chia sẻ trong các kênh riêng tư có hỗ trợ.

**Bạn cần một chủ sở hữu nhóm mới?**

Nếu chủ sở hữu kênh riêng của bạn rời khỏi, bạn có thể thêm chủ sở hữu nhóm mới qua teams PowerShell.


- Truy cập vào [đây](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) để cài đặt đội PowerShell.

Đây là lệnh bạn sẽ cần:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Để biết thêm thông tin về teams PowerShell, xem [tổng quan về nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
