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
ms.openlocfilehash: fa0e2766e1526d8e81cb247029e7c0fd98630b96
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316840"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP điểm cuối không được triển khai đến thiết bị của người dùng

Nếu thiết đặt Ngăn mất dữ liệu điểm cuối (DLP) chưa được áp dụng cho thiết bị của người dùng, hãy xác nhận rằng bạn đáp ứng các yêu cầu sau:

- Windows 10 cài đặt x64 bản dựng 1809 trở lên trên thiết bị.
- Đã cài đặt phiên bản máy khách chống phần mềm xấu phiên bản 4.18.2009.7 trở lên.
- Thiết bị là một **trong những** thiết bị sau:
    
    - Azure Active Directory (Azure AD) đã tham gia
    - Đã kết hợp Azure AD
    - Đã đăng ký AAD

- Để thực thi các hành động chính sách, hãy đảm bảo rằng Chromium duyệt Microsoft Edge được cài đặt trên thiết bị điểm cuối.

Để biết thêm yêu cầu về việc triển khai DLP Điểm cuối, hãy [xem Bắt đầu với ngăn mất dữ liệu Điểm cuối](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).