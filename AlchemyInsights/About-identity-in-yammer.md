---
title: Giới thiệu về căn cước trong Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918959"
---
# <a name="about-identity-in-yammer"></a>Giới thiệu về căn cước trong Yammer

Chúng tôi khuyên tất cả các mạng nên thực hiện các bước sau để tránh các sự cố liên quan đến danh tính:

1. Thực thi Office 365 nhận dạng sau khi cung cấp Microsoft 365 khoản người dùng trong Azure AD để đảm bảo rằng tất cả người dùng đăng nhập bằng cách sử dụng tài khoản Microsoft 365 chính của họ. Để biết thêm thông tin, hãy [xem phần Thực thi Office 365 nhận dạng cho Yammer người dùng.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Hợp nhất nhiều mạng Yammer khác nhau. Các cấu Yammer kế thừa cho phép Yammer nhiều mạng công cộng được kết nối với một đối tượng thuê. Để biết thêm thông tin, [xem mục Di chuyển mạng - Hợp nhất Yammer mạng.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Hoặc, bắt buộc cấp phép cho Yammer chặn người dùng khỏi Yammer nếu họ không có giấy phép. Để biết thêm thông tin, [hãy xem quản lý Yammer phép người dùng trong Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Cuối cùng, kiểm tra danh sách người dùng cho mạng Yammer cũ và tạm ngừng người dùng thừa tự. Chúng tôi khuyên bạn nên tạm ngừng người dùng (hủy kích hoạt) thay vì xóa họ, vì việc xóa không thể hoàn tác. Để biết thêm thông tin, hãy [xem mục Kiểm Yammer người dùng trong mạng được kết nối Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) và Loại bỏ người [dùng.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Bằng cách đặt cấu hình cho Yammer các bước này, bạn cũng sẽ sẵn sàng để đặt cấu hình mạng Yammer cho Chế độ Gốc cho máy Microsoft 365. Để biết thêm thông tin, hãy [xem mục Đặt cấu hình mạng Yammer của bạn cho Chế độ Gốc Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)