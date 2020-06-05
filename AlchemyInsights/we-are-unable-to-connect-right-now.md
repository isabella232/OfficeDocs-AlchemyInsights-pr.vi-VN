---
title: Vấn đề kích hoạt-chúng tôi không thể kết nối ngay bây giờ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581897"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Sửa chữa các ứng dụng Microsoft 365 "chúng tôi không thể kết nối ngay bây giờ" tin nhắn

Nếu bạn nhận được thông báo này, hãy thử như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet tới các ứng dụng Microsoft 365. Xem [các URL của Microsoft và các phạm vi địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Đi tới **bắt đầu**  >  **chạy**, và sau đó gõ **Services. msc**. Đảm bảo rằng các dịch vụ sau đang chạy:
    - Cài đặt tự động thiết bị kết nối mạng
    - Dịch vụ danh sách mạng
    - Nhận thức về vị trí mạng
    - Nhật ký sự kiện Windows

Nếu một trong các dịch vụ này không chạy, hãy thử khởi động nó. Nếu bạn gặp sự cố khởi động dịch vụ, chạy lệnh sau bằng cách mở dấu nhắc lệnh với quyền nâng cao:

**sfc/scannow**

Sau khi lệnh này kết thúc, khởi động lại máy tính.

Để biết thông tin chi tiết, xem ["xin lỗi, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau "lỗi khi bạn kích hoạt Office từ Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).