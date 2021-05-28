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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696980"
---
# <a name="11-call-recording"></a>Ghi âm cuộc gọi 1:1

Nếu nút **Bắt đầu Ghi** bị mờ trong cuộc gọi 1:1, bạn cần thay đổi cài đặt chính sách cho người dùng bị ảnh hưởng.   

Bắt đầu từ ngày 31 tháng 5 năm 2021, chúng tôi sẽ bắt đầu thực thi một Chính sách Gọi điện Teams *mới AllowCloudRecordingForCalls*. Trước thay đổi này, việc ghi lại cuộc gọi 1:1 được kiểm soát bởi Chính sách *Cho* phép Ghi Teams họp. Thay đổi này được ghi trong bài đăng trong Trung tâm Thông báo: [(Đã cập nhật) 1:1 Giới thiệu chính sách ghi âm cuộc gọi](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   tùy chọn chính sách cuộc gọi được đặt **thành $False** định. Nếu bạn muốn chặn tất cả người dùng khỏi bản ghi cuộc gọi 1:1, bạn không cần thực hiện bất kỳ hành động nào.  

Để bật ghi âm cuộc gọi cho tất cả người dùng trong cuộc gọi 1:1, hãy sử Teams PowerShell để chạy lệnh ghép ngắn sau: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Ngoài ra, bạn có thể tạo một chính sách mới và đặt **-AllowCloudRecordingForCalls** **thành $true** và gán chính sách đó cho người dùng của bạn. 

Để biết thêm thông tin, hãy xem Mục Điều khiển Chính sách Ghi Âm Cuộc gọi [1:1 (Gần như!) Tại đây](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
