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
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527776"
---
# <a name="password-logs"></a>Nhật ký mật khẩu

**Tôi đang gặp sự cố khi truy nhập Nhật ký kiểm tra đặt lại mật khẩu**

Để khắc phục sự cố về quyền truy nhập vào Nhật ký kiểm tra đặt lại mật khẩu, hãy thực hiện bước sau đây:

Đảm bảo bạn được ủy quyền để xem Nhật ký kiểm nghiệm. 

Chỉ những vai trò sau đây được ủy quyền:
 - Người quản trị toàn cầu
 - Người quản trị bảo mật
 - Bộ đọc bảo mật

**Tôi muốn xem tất cả các sự kiện kiểm tra khôi phục mật khẩu từ lúc tôi triển khai ban đầu**

Lên đến 120.000 đặt lại mật khẩu/sự kiện đăng ký được lưu trữ trong các báo cáo của 30 ngày qua. Giới hạn tối đa này áp dụng cho giao diện người dùng khi tải xuống CSV. sự kiện 1.000.000 sẵn dùng thông qua PowerShell.
Để biết thêm thông tin, hãy xem các nối kết dưới đây:

- [Tự khôi phục mật khẩu các sự kiện từ Azure AD Reports and events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Làm thế nào để tải lại các sự kiện đăng ký mật khẩu nhanh chóng với PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Tôi muốn tìm hiểu thêm về các chức năng báo cáo đặt lại mật khẩu**

Kiểm tra xem ai đang đăng ký hoặc đặt lại mật khẩu có Nhật ký kiểm tra khôi phục mật khẩu Azure AD trong cổng thông tin Azure bên dưới **người dùng và nhóm**.
Để biết thêm thông tin, hãy xem các nối kết sau đây:

- [Tổng quan về báo cáo đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cách xem báo cáo đặt lại mật khẩu trong cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Tự khôi phục mật khẩu các sự kiện từ Azure AD Reports and events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Làm thế nào để tải lại các sự kiện đăng ký mật khẩu nhanh chóng với PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


