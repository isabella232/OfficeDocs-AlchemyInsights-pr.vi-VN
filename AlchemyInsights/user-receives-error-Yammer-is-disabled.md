---
title: Người dùng nhận được lỗi Truy nhập AADSTS7000112 Yammer tắt
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
ms.openlocfilehash: f2e23d63338ece5332ad4fd2b2d59021eb45d9bf32632d3cc23089c919d4e402
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971253"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Người dùng nhận được lỗi Truy nhập AADSTS7000112 Yammer tắt

Nếu bạn nhận được lỗi "AADSTS7000112: Ứng dụng '000000005-0000-0ff1-ce00-000000000000'(Yammer) bị vô hiệu hóa", một sự cố xảy ra với tài khoản dịch vụ chính trong Azure AD. Người quản trị có thể đã tắt tài khoản chính của dịch vụ để chặn quyền truy nhập vào Yammer.

Chúng tôi khuyên bạn không nên vô hiệu hóa tài khoản dịch vụ chính và có thể gây ra sự cố bổ sung. Để biết thêm thông tin về các phương pháp được hỗ trợ để chặn quyền truy nhập người dùng vào Yammer, hãy xem Tắt quyền truy [Yammer nhập của người Microsoft 365 người dùng.](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)  

Để khắc phục sự cố này trong Cổng thông tin Azure và khôi phục quyền truy nhập người dùng vào Yammer:

1.  Mở trang Azure Active Directory, rồi chọn Ứng dụng doanh **nghiệp bên** dưới **Quản lý** trong ngăn dẫn hướng bên trái.
3.  Nhập **Office 365 Yammer** vào hộp tìm kiếm, rồi chọn tên ứng dụng để mở cài đặt.
4.  Chọn **Thuộc tính** bên dưới **Quản** lý trong ngăn dẫn hướng bên trái.
5.  Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.
6.  Đăng nhập vào Yammer lần nữa. Bạn có thể cần xóa cookie.

Ngoài ra, hãy chạy các lệnh PowerShell để đặt giá trị. Để biết thêm thông tin, hãy xem lỗi ["Rất tiếc,](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn" khi bạn bấm vào ô Yammer trong Office 365. 