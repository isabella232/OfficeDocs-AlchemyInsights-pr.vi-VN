---
title: Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hóa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796670"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hóa

Nếu bạn nhận được lỗi "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (yammer) bị vô hiệu hóa", vấn đề này tồn tại với hiệu trưởng dịch vụ trong Azure AD. Người quản trị có thể đã vô hiệu hóa hiệu trưởng dịch vụ để chặn quyền truy nhập vào yammer.

Vô hiệu hóa hiệu trưởng của dịch vụ không được đề xuất và có thể gây ra sự cố bổ sung. Để biết thêm thông tin về cách tiếp cận được hỗ trợ để chặn quyền truy nhập của người dùng vào yammer, hãy xem mục tắt [truy nhập yammer dành cho người dùng Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Để sửa vấn đề này trong cổng thông tin Azure và khôi phục quyền truy nhập của người dùng vào yammer:

1.  Mở trang Azure Active Directory, rồi chọn các **ứng dụng doanh nghiệp** bên dưới **quản lý** trong ngăn dẫn hướng bên trái.
3.  Nhập **Office 365 yammer** trong hộp tìm kiếm, rồi chọn tên ứng dụng để mở thiết đặt.
4.  Chọn **thuộc tính** bên dưới **quản lý** trong ngăn dẫn hướng bên trái.
5.  Đặt giá trị được **kích hoạt cho người dùng đăng nhập?** để **có**, rồi chọn **lưu**.
6.  Đăng nhập lại vào yammer. Bạn có thể cần xóa các cookie.

Ngoài ra, hãy chạy lệnh PowerShell để đặt giá trị. Để biết thêm thông tin, hãy xem mục ["rất tiếc nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn trong" lỗi khi bạn bấm vào lát xếp yammer trong Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 