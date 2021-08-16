---
title: Sự cố Kích hoạt - Chúng tôi không thể kết nối ngay bây giờ
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998194"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Khắc phục sự cố thông báo Microsoft 365 "Chúng tôi không thể kết nối ngay bây giờ"

Nếu bạn nhận được thông báo này, hãy thử làm như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy của bạn để xác nhận rằng họ không chặn truy nhập Internet vào các Microsoft 365 của bạn. Xem [URL Microsoft và dải địa chỉ IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Đi tới **Bắt**  >  **đầu Chạy**, sau đó nhập **services.msc**. Đảm bảo rằng tất cả các dịch vụ sau đều đang chạy:
    - Tự động Thiết lập Thiết bị Đã kết nối Mạng
    - Dịch vụ Danh sách Mạng
    - Nhận thức về Vị trí Mạng
    - Windows Nhật ký Sự kiện

Nếu một trong các dịch vụ này không chạy, hãy thử khởi động lại. Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau đây bằng cách mở dấu nhắc lệnh có các quyền mức cao:

**sfc /scannow**

Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.

Để biết thông tin chi tiết, [hãy xem mục "Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau" khi bạn kích hoạt Office từ máy Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)