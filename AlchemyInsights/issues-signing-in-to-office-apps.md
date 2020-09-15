---
title: Các sự cố khi đăng nhập vào ứng dụng Microsoft 365
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695345"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Khắc phục sự cố cho ứng dụng Microsoft 365 "rất tiếc, một tài khoản khác từ tổ chức của bạn đã được đăng nhập"

Để khắc phục lỗi này, hãy thử làm như sau:

- Loại bỏ tất cả tài khoản công việc, ngoại trừ tài khoản bị ảnh hưởng, bằng cách sử dụng thiết đặt Windows > **truy nhập công việc hoặc trường học**.
- [Xóa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mở một ứng dụng Office, **File**chọn đăng xuất  >  **tài khoản**tệp  >  **Sign Out**. Sau đó, đăng nhập bằng tài khoản người dùng với giấy phép hợp lệ. Để biết thông tin chi tiết, hãy xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Đối với máy Mac, hãy xem [không thể đăng nhập vào ứng dụng Office 2016 cho Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Để biết thêm thông tin, hãy xem ["xin lỗi, tài khoản khác từ tổ chức của bạn đã được đăng nhập trên máy tính này" trong Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).