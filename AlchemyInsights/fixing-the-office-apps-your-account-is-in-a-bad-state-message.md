---
title: Sửa chữa các ứng dụng văn phòng tài khoản của bạn đang ở trạng thái xấu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969935"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Sửa chữa các ứng dụng Office "tài khoản của bạn đang ở trạng thái xấu" lỗi

Để khắc phục lỗi này, hãy thử các tuỳ chọn sau trên máy tính bị ảnh hưởng:

- Mở ứng dụng Office, chọn **** > **tài khoản** > tệp**đăng xuất khỏi tất cả tài khoản**. Đăng nhập lại bằng tài khoản người dùng có giấy phép hợp lệ. Để biết thông tin chi tiết, xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.<br>
  **Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0. Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\
- Trên máy tính bị ảnh hưởng, đặt EnableADAL = 0 bằng cách sử dụng các bước sau:  
     1. Bấm chuột phải vào nút Windows và chọn **chạy**. Trong hộp **mở** , gõ **regedit**, và sau đó chọn **OK**.
     2. Chọn **có** khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.
    3. Trong trình chỉnh sửa sổ đăng ký, thêm giá trị EnableADAL với thiết đặt 0 trong HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Nếu xảy ra lỗi khi kết nối với Office 365 bằng cách sử dụng Office 2013, [kích hoạt xác thực hiện đại](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) cho khách hàng Office.

Để biết thêm thông tin, hãy xem [cách khắc phục sự cố ứng dụng không có trình duyệt không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

