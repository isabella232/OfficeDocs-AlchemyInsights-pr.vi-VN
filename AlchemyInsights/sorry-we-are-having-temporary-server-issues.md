---
title: Khắc phục sự cố ứng dụng Microsoft 365 rất tiếc, chúng tôi có thông báo vấn đề máy chủ tạm thời
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758267"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Sửa lỗi ứng dụng Microsoft 365 "rất tiếc, chúng tôi đang gặp phải sự cố máy chủ tạm thời"

Nếu bạn nhận được thông báo này, hãy thử làm như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không chặn truy nhập Internet vào các ứng dụng Microsoft 365. Xem [dải URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Đi đến **bắt đầu**  >  **chạy**, rồi nhập **Services. msc**. Hãy đảm bảo rằng các dịch vụ sau đây đều đang chạy:
    - Thiết lập tự động thiết bị kết nối mạng
    - Dịch vụ danh sách mạng
    - Nâng cao vị trí mạng
    - Nhật ký sự kiện Windows

Nếu một trong các dịch vụ này không chạy, hãy thử khởi động ứng dụng này. Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau bằng cách mở dấu nhắc lệnh với các quyền tăng cao:

**sfc/scannow**

Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.

Để biết thông tin chi tiết, hãy xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi" khi bạn kích hoạt](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).