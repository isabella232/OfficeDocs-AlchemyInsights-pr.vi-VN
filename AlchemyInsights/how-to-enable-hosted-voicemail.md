---
title: Cách bật Thư thoại Đã lưu
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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318670"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cách bật Thư thoại Đã lưu

Để bật Thư thoại, **phải đặt HostedVoicemail** thành Thư $true.

Thuộc **tính HostedVoicemail** trên người dùng bằng cách sử dụng Remote PowerShell (RPS).

Để biết thêm thông tin về việc kết nối với RPS, hãy [Microsoft Teams Tổng quan về PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) để biết thêm thông tin về việc kết nối với RPS.

1. Người quản Teams cần được đăng nhập vào Remote PowerShell for Teams.
1. Từ PowerShell, hãy nhắc Người quản trị Teams có thể chạy **set-csuser user@contoso.com -HostedVoiceMail $true** trong đó uri sip là của người dùng được đề cập.

**Lưu** ý : Bạn có thể phải mất tới 24 giờ để thay đổi các chính sách.