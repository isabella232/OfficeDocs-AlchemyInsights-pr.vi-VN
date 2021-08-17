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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055576"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cách bật Thư thoại Đã lưu

Để bật Thư thoại, **phải đặt HostedVoicemail** thành Thư $true.

Thuộc **tính HostedVoicemail** trên người dùng bằng cách sử dụng Remote PowerShell (RPS).

Để biết thêm thông tin về việc kết nối với RPS, hãy [Microsoft Teams Tổng quan về PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) để biết thêm thông tin về việc kết nối với RPS.

1. Người quản Teams cần được đăng nhập vào Remote PowerShell for Teams.
1. Từ PowerShell, hãy nhắc Người quản Teams có thể chạy **set-csuser user@contoso.com -HostedVoiceMail $true** trong đó uri sip là của người dùng được đề cập.

> [!NOTE]
> Thay đổi đối với chính sách có thể mất đến 24 giờ để nhân bản.