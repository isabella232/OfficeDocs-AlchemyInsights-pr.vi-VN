---
title: Ghi âm cuộc gọi 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314406"
---
# <a name="11-call-recording"></a>Ghi âm cuộc gọi 1:1

Nếu nút **Bắt đầu Ghi** bị mờ trong cuộc gọi 1:1, bạn cần thay đổi cài đặt chính sách cho người dùng bị ảnh hưởng. Để kiểm tra cài đặt chính sách, hãy chạy Chẩn đoán cho người dùng bị ảnh hưởng bằng cách nhập **Diag: Teams 1:1 Ghi Âm Cuộc gọi ở** trên.     

Bắt đầu từ ngày 31 tháng 5 năm 2021, chúng tôi sẽ bắt đầu thực thi một Chính sách Gọi điện Teams *mới AllowCloudRecordingForCalls*. Trước thay đổi này, bản ghi cuộc gọi 1:1 được kiểm soát bởi Chính sách *Cho* phép Ghi Teams Họp. Thay đổi này được ghi lại trong bài đăng của Trung tâm Thông báo: [(Đã cập nhật) 1:1 Giới thiệu chính sách ghi âm cuộc gọi](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   tùy chọn chính sách cuộc gọi được đặt **thành $False** định. Nếu bạn muốn chặn tất cả người dùng khỏi bản ghi cuộc gọi 1:1, bạn không cần thực hiện bất kỳ hành động nào.  

Để bật ghi âm cuộc gọi cho tất cả người dùng trong cuộc gọi 1:1, hãy [sử Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) để chạy lệnh ghép ngắn sau: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Ngoài ra, bạn có thể tạo một chính sách mới và đặt **-AllowCloudRecordingForCalls** **thành $true** và gán chính sách đó cho người dùng của bạn. 

Để biết thêm thông tin, hãy xem Mục Điều khiển Chính sách Ghi Âm Cuộc gọi [1:1 (Gần như!) Tại đây](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
