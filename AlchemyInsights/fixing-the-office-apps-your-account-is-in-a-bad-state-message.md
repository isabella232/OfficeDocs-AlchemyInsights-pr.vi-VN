---
title: Khắc phục các ứng dụng Microsoft 365 tài khoản của bạn nằm trong một thông điệp trạng thái xấu
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744567"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Sửa lỗi ứng dụng Microsoft 365 "tài khoản của bạn đang ở trạng thái trạng thái xấu"

Để khắc phục lỗi này, hãy thử các tùy chọn sau trên máy tính bị ảnh hưởng:

- Mở một ứng dụng Office, **File**chọn  >  đăng nhập**tài khoản**tệp  >  **khỏi tất cả các tài khoản**. Đăng nhập lại bằng tài khoản người dùng với giấy phép hợp lệ. Để biết thông tin chi tiết, hãy xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Xóa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.<br>
  **Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0. Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\
- Nếu lỗi xảy ra trong khi kết nối với Office 365 bằng Office 2013, hãy [bật xác thực hiện đại](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) cho máy khách Office.

Để biết thêm thông tin, hãy xem [cách khắc phục sự cố các ứng dụng không phải trình duyệt không thể đăng nhập vào Microsoft 365, Azure hoặc InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

