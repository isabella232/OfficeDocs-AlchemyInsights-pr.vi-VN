---
title: Về danh tính trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148422"
---
# <a name="about-identity-in-yammer"></a>Về danh tính trong yammer

Đó là khuyến cáo rằng tất cả các mạng thực hiện các bước sau để tránh các vấn đề liên quan đến danh tính:

1. Thực thi Office 365 nhận dạng sau khi cung cấp tài khoản Microsoft 365 cho người dùng Azure AD để đảm bảo rằng tất cả người dùng đăng nhập bằng cách sử dụng tài khoản Microsoft 365 chính. Để biết thêm thông tin, xem [thi hành Office 365 nhận dạng cho người dùng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Củng cố nhiều yammer mạng. Cấu hình kế thừa yammer cho phép nhiều mạng yammer được kết nối với một đối tượng thuê. Để biết thêm thông tin, xem [di chuyển mạng-hợp nhất nhiều yammer mạng](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Tùy chọn, thực thi cấp phép cho yammer để chặn người dùng từ yammer nếu họ không có giấy phép. Để biết thêm thông tin, xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Cuối cùng, kiểm tra danh sách người dùng cho mạng yammer cũ và tạm ngưng người dùng hợp lệ. Chúng tôi đề nghị bạn tạm ngưng (Hủy kích hoạt) người dùng thay vì xóa chúng, vì xóa là không thể đảo ngược. Để biết thêm thông tin, xem [kiểm tra yammer người dùng trong mạng kết nối với Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) và [loại bỏ người dùng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Bằng cách đặt cấu hình yammer bằng các bước này, bạn cũng sẽ sẵn sàng cấu hình mạng yammer cho chế độ riêng dành cho Microsoft 365. Để biết thêm thông tin, hãy xem [cấu hình mạng yammer của bạn cho chế độ riêng cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).