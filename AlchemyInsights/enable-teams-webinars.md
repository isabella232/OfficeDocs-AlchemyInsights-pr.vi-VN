---
title: Bật Hội Teams Web
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794034"
---
# <a name="enable-teams-webinars"></a>Bật Hội Teams Web

Hội thảo trên web được bật theo mặc định. Bạn có thể quản lý những người có thể lên lịch và đăng ký Teams Webinars bằng cách Teams lệnh PowerShell.

- Tất cả người dùng có thể tạo cuộc họp cũng có thể tạo cuộc họp hội thảo web. Nếu bạn muốn quản lý những người có thể lên lịch Teams Webinars, hãy sử *dụng AllowMeetingRegistration*. 
- Theo mặc định, *WhoCanRegister* được bật và đặt là Mọi **người**. Nếu bạn muốn tắt tính năng đăng ký cuộc họp, hãy *đặt AllowMeetingRegistration* thành **False.**

Để thay đổi các thiết đặt này, bạn [phải cài Teams PowerShell](/microsoftteams/teams-powershell-install). Ngoài ra, Chính sách Cuộc họp được thực thi Teams Webinars. Ví dụ: nếu kết nối ẩn danh bị tắt trong thiết đặt cuộc họp thì người dùng ẩn danh sẽ không thể tham gia hội thảo web.

Để tìm hiểu thêm về việc đặt cấu hình những người có thể đăng ký hội thảo trên web, hãy xem mục Đặt cấu hình những người có thể đăng [ký hội thảo trên web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Để biết thêm thông tin về các cài đặt cho Danh sách Microsoft, hãy xem [Mục Kiểm soát cài đặt cho Danh sách Microsoft](/sharepoint/control-lists).