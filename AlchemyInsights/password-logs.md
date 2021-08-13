---
title: Nhật ký mật khẩu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960965"
---
# <a name="password-logs"></a>Nhật ký mật khẩu

**Tôi đang gặp sự cố khi truy nhập nhật ký kiểm tra đặt lại mật khẩu**

Để khắc phục sự cố về quyền truy nhập vào nhật ký kiểm tra đặt lại mật khẩu, hãy thực hiện các bước sau đây:

Đảm bảo bạn được phép xem nhật ký kiểm tra. 

Chỉ những vai trò sau đây được ủy quyền:
 - Người quản trị toàn cầu
 - Người quản trị bảo mật
 - Bộ đọc bảo mật

**Tôi muốn xem tất cả các sự kiện kiểm tra đặt lại mật khẩu kể từ thời điểm tôi triển khai lần đầu**

Tối đa 120.000 sự kiện đặt lại/đăng ký mật khẩu sẽ được lưu trữ trong báo cáo về 30 ngày gần nhất. Giới hạn tối đa này áp dụng cho giao diện người dùng khi tải xuống CSV. 1 triệu sự kiện sẽ sẵn dùng thông qua PowerShell.
Để biết thêm thông tin, hãy xem các liên kết dưới đây:

- [Các sự kiện tự đặt lại mật khẩu từ API Báo cáo và Sự kiện Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cách nhanh chóng tải xuống các sự kiện đăng ký đặt lại mật khẩu với PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Tôi muốn tìm hiểu thêm về chức năng báo cáo đặt lại mật khẩu**

Kiểm tra xem ai đang đăng ký hoặc đặt lại mật khẩu bằng nhật ký kiểm tra đặt lại mật khẩu Azure AD trong cổng thông tin Azure **bên dưới Người dùng và nhóm.**
Để biết thêm thông tin, hãy xem các nối kết sau đây:

- [Tổng quan về đặt lại báo cáo bằng mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cách xem báo cáo đặt lại mật khẩu trong cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Các sự kiện tự đặt lại mật khẩu từ API Báo cáo và Sự kiện Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cách nhanh chóng tải xuống các sự kiện đăng ký đặt lại mật khẩu với PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


