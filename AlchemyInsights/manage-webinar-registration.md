---
title: Quản lý đăng ký hội thảo web
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798666"
---
# <a name="manage-webinar-registration"></a>Quản lý đăng ký hội thảo web

Bạn quản lý những người có thể đăng ký Teams Webinars bằng cách sử Teams lệnh Powershell mới. Để cài Teams Powershell, hãy [xem Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Theo mặc định, *WhoCanRegister* được bật và đặt là Mọi **người**. 

Nếu bạn không thấy tùy chọn cho phép đăng ký cho Mọi người trong thư mời họp, hãy chạy lại cài đặt *WhoCanRegister* to Everyone và chờ 24 giờ. Để chạy lại *WhoCanRegister*, hãy sử dụng lệnh Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Lưu ý:** Nếu tham gia ẩn danh được tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web. Để tìm hiểu thêm và bật thiết đặt này, hãy [xem Quản lý thiết đặt cuộc họp Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**

Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).
