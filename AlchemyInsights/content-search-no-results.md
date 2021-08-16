---
title: Tìm kiếm Nội dung Không có Kết quả
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058024"
---
# <a name="no-results-from-content-searchexports"></a>Không có kết quả nào từ Tìm kiếm/Xuất Nội dung

Sự cố với Tìm kiếm/Xuất Nội dung không trả về bất kỳ dữ liệu nào có thể là do một Bộ lọc Bảo mật Tuân thủ nhất định đã được một Người quản trị cụ thể thiết lập và không thông báo cho tất cả người quản trị.

Để giải quyết vấn đề này, hãy kiểm tra xem liệu có bất kỳ Bộ lọc Bảo mật Tuân thủ nào mà có thể gây ra vấn đề này không:
1. Kết nối powershell của Trung tâm Bảo mật và Tuân thủ
2. Chạy lệnh dưới đây:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Trợ lý Tổ chức $org