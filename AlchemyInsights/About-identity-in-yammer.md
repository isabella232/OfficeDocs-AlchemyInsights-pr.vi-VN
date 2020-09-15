---
title: Giới thiệu về danh tính trong yammer
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
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664192"
---
# <a name="about-identity-in-yammer"></a>Giới thiệu về danh tính trong yammer

Khuyên rằng tất cả các mạng sẽ thực hiện các bước sau đây để tránh các vấn đề liên quan đến căn cước:

1. Áp dụng định danh Office 365 sau khi cung cấp tài khoản Microsoft 365 cho người dùng trong Azure AD để đảm bảo rằng tất cả người dùng đăng nhập bằng tài khoản Microsoft 365 chính của họ. Để biết thêm thông tin, hãy xem thực [thi định danh Office 365 cho người dùng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Hợp nhất nhiều mạng yammer. Cấu hình yammer kế thừa cho phép nhiều mạng yammer được kết nối với một đối tượng thuê. Để biết thêm thông tin, hãy xem mục [di chuyển mạng-hợp nhất nhiều mạng yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Bạn có thể thực thi cấp phép cho yammer để chặn người dùng từ yammer nếu họ không có giấy phép. Để biết thêm thông tin, hãy xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Cuối cùng, hãy kiểm tra danh sách người dùng cho mạng yammer cũ hơn và tạm ngừng người dùng thừa kế. Bạn nên tạm ngừng (Hủy kích hoạt) người dùng thay vì xóa chúng, vì việc xóa bỏ không thể thay đổi. Để biết thêm thông tin, hãy xem [kiểm tra người dùng yammer trong các mạng được kết nối với Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) và [loại bỏ người dùng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Bằng cách đặt cấu hình yammer bằng các bước này, bạn cũng sẽ sẵn sàng cấu hình mạng yammer của bạn cho chế độ bản địa cho Microsoft 365. Để biết thêm thông tin, hãy xem [đặt cấu hình mạng yammer của bạn cho chế độ bản địa cho Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).