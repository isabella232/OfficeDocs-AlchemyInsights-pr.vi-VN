---
title: Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hoá
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198366"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hoá

Nếu bạn nhận được lỗi "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (yammer) bị vô hiệu hoá", sự cố tồn tại với các dịch vụ chính trong Azure quảng cáo. Quản trị viên có thể đã vô hiệu hoá dịch vụ chính để chặn truy cập vào yammer.

Vô hiệu hoá dịch vụ chính không được khuyến nghị và có thể gây ra sự cố khác. Để biết thêm thông tin về phương pháp được hỗ trợ để chặn người dùng truy cập vào yammer, [hãy xem tắt truy cập yammer cho người dùng Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Để khắc phục sự cố này trong cổng thông tin Azure và quyền truy cập của người dùng vào yammer:

1.  Mở trang Azure Active Directory và chọn **ứng dụng doanh nghiệp** trong **quản lý** trong ngăn điều hướng bên trái.
3.  Nhập **Office 365 yammer** vào hộp tìm kiếm, và chọn tên ứng dụng để mở cài đặt.
4.  Chọn thuộc **tính** trong **quản lý** trong ngăn điều hướng bên trái.
5.  Đặt giá trị **cho phép người dùng đăng nhập?** **có**, và sau đó chọn **lưu**.
6.  Đăng nhập lại vào yammer. Bạn có thể cần phải xóa cookie.

Ngoài ra, chạy lệnh PowerShell để đặt giá trị. Để biết thêm thông tin, hãy xem ["xin lỗi, nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn vào" lỗi nếu bạn bấm vào ngăn xếp yammer trong Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 