---
title: Khắc phục sự Microsoft 365 rất tiếc, thông báo Sự cố máy chủ tạm thời
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021618"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Khắc phục sự cố thông báo Microsoft 365 "Rất tiếc, chúng tôi đang gặp phải sự cố máy chủ tạm thời"

Nếu bạn nhận được thông báo này, hãy thử làm như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy của bạn để xác nhận rằng họ không chặn truy nhập Internet vào các Microsoft 365 của bạn. Xem [URL và dải địa chỉ IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Đi tới **Bắt**  >  **đầu Chạy**, sau đó nhập **services.msc**. Đảm bảo rằng tất cả các dịch vụ sau đều đang chạy:
    - Tự động Thiết lập Thiết bị Đã kết nối Mạng
    - Dịch vụ Danh sách Mạng
    - Nhận thức về Vị trí Mạng
    - Windows Nhật ký Sự kiện

Nếu một trong các dịch vụ này không chạy, hãy thử khởi động lại. Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau đây bằng cách mở dấu nhắc lệnh có các quyền mức cao:

**sfc /scannow**

Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.

Để biết thông tin chi tiết, [hãy xem mục "Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Lỗi vui lòng thử lại sau" khi bạn kích hoạt](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).