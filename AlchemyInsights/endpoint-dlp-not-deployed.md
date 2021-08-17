---
title: DLP điểm cuối không được triển khai đến thiết bị của người dùng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 2d5f0486ed8d4cbd95603f223bc0e48c4dcf38abb001d1616ca968b1d6bba7de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044254"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP điểm cuối không được triển khai đến thiết bị của người dùng

Nếu thiết đặt Ngăn mất dữ liệu điểm cuối (DLP) chưa được áp dụng cho thiết bị của người dùng, hãy xác nhận rằng bạn đáp ứng các yêu cầu sau:

- Windows 10 bản x64 bản dựng 1809 trở lên đã được cài đặt trên thiết bị.
- Đã cài đặt phiên bản máy khách chống phần mềm xấu phiên bản 4.18.2009.7 trở lên.
- Thiết bị là một **trong những thiết** bị sau:
    
    - Azure Active Directory (Azure AD) đã tham gia
    - Đã kết hợp Azure AD
    - Đã đăng ký AAD

- Để thực thi các hành động chính sách, hãy đảm bảo Chromium Microsoft Edge được cài đặt trên thiết bị điểm cuối.

Để biết thêm yêu cầu về việc triển khai DLP Điểm cuối, hãy [xem Bắt đầu với ngăn mất dữ liệu Điểm cuối](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).