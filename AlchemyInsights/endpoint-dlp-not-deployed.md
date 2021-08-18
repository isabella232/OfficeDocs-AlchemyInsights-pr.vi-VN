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
ms.openlocfilehash: 56783b007b5eebc7ca671247f24f5b513b9d8f5c321f59a63170425c2d376a94
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900270"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP điểm cuối không được triển khai đến thiết bị của người dùng

Nếu thiết đặt Ngăn mất dữ liệu điểm cuối (DLP) chưa được áp dụng cho thiết bị của người dùng, hãy xác nhận rằng bạn đáp ứng các yêu cầu sau:

- Windows 10 cài đặt trên thiết bị bằng x64 bản dựng 1809 trở lên.
- Đã cài đặt phiên bản máy khách chống phần mềm xấu phiên bản 4.18.2009.7 trở lên.
- Thiết bị là một **trong những** thiết bị sau:
    
    - Azure Active Directory (Azure AD) đã tham gia
    - Đã kết hợp Azure AD
    - Đã đăng ký AAD

- Để thực thi các hành động chính sách, hãy đảm bảo Chromium Microsoft Edge được cài đặt trên thiết bị điểm cuối.

Để biết thêm yêu cầu về việc triển khai DLP Điểm cuối, hãy [xem Bắt đầu với ngăn mất dữ liệu Điểm cuối](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).