---
title: Các sự cố khi đăng nhập vào ứng dụng Microsoft 365
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833097"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Khắc phục sự cố cho ứng dụng Microsoft 365 "rất tiếc, một tài khoản khác từ tổ chức của bạn đã được đăng nhập"

Để khắc phục lỗi này, hãy thử làm như sau:

- Loại bỏ tất cả tài khoản công việc, ngoại trừ tài khoản bị ảnh hưởng, bằng cách sử dụng thiết đặt Windows > **truy nhập công việc hoặc trường học**.
- [Xóa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mở một ứng dụng Office, chọn đăng xuất  >  **tài khoản** tệp  >  . Sau đó, đăng nhập bằng tài khoản người dùng với giấy phép hợp lệ. Để biết thông tin chi tiết, hãy xem [tài khoản trong Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Đối với máy Mac, hãy xem [không thể đăng nhập vào ứng dụng Office 2016 cho Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Để biết thêm thông tin, hãy xem ["xin lỗi, tài khoản khác từ tổ chức của bạn đã được đăng nhập trên máy tính này" trong Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).