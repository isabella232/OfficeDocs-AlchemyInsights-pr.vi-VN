---
title: bản ghi cuộc gọi 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733871"
---
# <a name="11-call-recording"></a>bản ghi cuộc gọi 1:1

Người quản trị cần thực hiện hành động để tiếp tục cho phép người dùng ghi lại cuộc gọi 1:1.
 
Bắt đầu từ ngày 12/04/2018, 2021, chúng tôi sẽ bắt đầu thực thi tùy chọn chính sách gọi nhóm mới trong *Allowcloudrecordingforcalls*. 

Hiện tại, các chức năng ghi cuộc gọi 1:1 được điều khiển bởi tùy chọn *Allowcloudrecording* trong chính sách cuộc họp nhóm. Nếu người dùng của bạn được phép ghi lại cuộc họp nhóm, họ cũng có thể ghi lại các cuộc gọi 1:1.

Nếu bạn muốn chặn tất cả người dùng ghi lại cuộc gọi 1:1, bạn không cần thực hiện bất kỳ hành động nào. Tùy chọn chính sách gọi cho *Allowcloudrecordingforcalls* sẽ được $false theo mặc định.

Thay đổi này được tài liệu trong bài đăng của Trung tâm thông báo sau: [(Cập Nhật) 1:1 gọi giới thiệu chính sách ghi âm](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) để đặt tùy chọn chính sách gọi nhóm, bạn phải sử dụng [nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Để bật ghi cuộc gọi trong 1:1 cuộc gọi:** Set-CsTeamsCallingPolicy-căn cước cho các cuộc gọi toàn cầu-Allowcloudrecording$True

**Để tắt tính năng ghi cuộc gọi trong 1:1 cuộc gọi:** Set-CsTeamsCallingPolicy-căn cước các cuộc gọi toàn cầu-allowcloudtheo $false

