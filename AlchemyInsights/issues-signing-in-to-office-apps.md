---
title: Các sự cố về đăng nhập vào Microsoft 365 dụng
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
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028062"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Khắc phục sự cố Microsoft 365 thông báo "Rất tiếc, một tài khoản khác từ tổ chức của bạn đã đăng nhập"

Để khắc phục lỗi này, hãy thử cách sau:

- Loại bỏ tất cả tài khoản cơ quan, ngoại trừ tài khoản bị ảnh hưởng bằng cách Windows Cài đặt > **truy nhập tài khoản cơ quan hoặc trường học**.
- [Xóa thông Office tin xác thực](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách Windows Trình quản lý chứng danh.<br/>
    **Lưu ý:** Đường dẫn sổ đăng ký Office 2016 đã thay đổi thành 16.0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Mở một tài Ứng dụng Office, chọn **Đăng**  >  **xuất Tài khoản**  >  **Tệp**. Sau đó, đăng nhập bằng tài khoản người dùng với giấy phép hợp lệ. Để biết thông tin chi tiết, [hãy xem Tài khoản Office.](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- Đối với máy Mac, [xem mục Không thể đăng nhập vào ứng dụng Office 2016 for Mac.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

Để biết thêm thông tin, hãy xem "Rất tiếc, một tài khoản khác từ tổ chức của bạn đã đăng nhập trên máy tính [này" trong Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)