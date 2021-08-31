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
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744617"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Khắc phục sự cố Microsoft 365 thông báo "Chúng tôi không thể kết nối ngay bây giờ"

Lưu ý: Nếu bạn đang sử dụng phiên bản cũ hơn của Windows (ví dụ: Windows 7 SP1, [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Windows Server 2008 R2), hãy sử dụng bản sửa lỗi dễ dàng để bật TLS 1.2 làm mặc định. Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)làm giao thức bảo mật mặc định trong WinHTTP Windows.

Nếu bạn nhận được thông báo này, hãy thử làm như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy của bạn để xác nhận rằng họ không chặn truy nhập Internet vào các Microsoft 365 dụng của bạn. Xem [URL Microsoft và dải địa chỉ IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Đi tới **Bắt**  >  **đầu Chạy**, sau đó nhập **services.msc**. Đảm bảo rằng tất cả các dịch vụ sau đều đang chạy:
    - Tự động Thiết lập Thiết bị Đã kết nối Mạng
    - Dịch vụ Danh sách Mạng
    - Nhận thức về Vị trí Mạng
    - Windows Nhật ký Sự kiện

Nếu một trong các dịch vụ này không chạy, hãy thử khởi động lại. Nếu bạn gặp sự cố khi bắt đầu dịch vụ, hãy chạy lệnh sau đây bằng cách mở dấu nhắc lệnh với quyền nâng cao:

**sfc /scannow**

Sau khi lệnh này kết thúc, hãy khởi động lại máy tính.

Để biết thông tin chi tiết, [hãy xem mục "Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau" khi bạn kích hoạt Office từ máy Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)