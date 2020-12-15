---
title: Cách bật thư thoại được lưu trữ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679160"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cách bật thư thoại được lưu trữ

Để bật thư thoại, **Hosteivoicemail** phải được đặt là $true.

Thuộc tính **Hostedvoicemail** trên người dùng bằng cách sử dụng Remote PowerShell (RPS).

Để biết thêm thông tin về kết nối đến RPS, hãy xem [tổng quan về Microsoft nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) để biết thêm thông tin về kết nối đến RPS.

1. Người quản trị nhóm phải được đăng nhập vào PowerShell từ xa cho các nhóm.
1. Từ PowerShell nhắc người quản trị nhóm có thể chạy **Set-csuser user@contoso.com-hostetin thư thoại $True** nơi mà URI SIP là người dùng trong câu hỏi.

> [!NOTE]
> Những thay đổi đối với các chính sách có thể mất tối đa 24 giờ để sao chép.