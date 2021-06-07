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
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794141"
---
# <a name="manage-webinar-registration"></a>Quản lý đăng ký hội thảo web

Bạn quản lý những người có thể đăng ký Teams Webinars bằng cách sử Teams lệnh Powershell mới. Để cài Teams Powershell, hãy [xem Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Theo mặc định, *WhoCanRegister* được bật và đặt thành **EveryoneInCompany**. Để cho phép bất kỳ ai, bao gồm người  dùng ẩn danh, đăng ký, bạn phải đặt Chính sách Cuộc họp cho Mọi người bằng cách sử dụng lệnh Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Lưu ý:** Nếu tham gia ẩn danh được tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web. Để tìm hiểu thêm và bật thiết đặt này, hãy [xem Quản lý thiết đặt cuộc họp Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**

Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).
