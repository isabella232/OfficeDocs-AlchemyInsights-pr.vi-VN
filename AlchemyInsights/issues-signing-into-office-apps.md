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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986913"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Thông báo Khắc Microsoft 365 "Mô-đun Nền tảng Tin cậy của máy tính của bạn không hoạt động đúng cách"

Để khắc phục lỗi này, hãy thử cách sau:

- Cài đặt các bản cập nhật mới [nhất cho Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Xóa thông Office tin xác thực](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) bằng cách Windows Trình quản lý chứng danh.<br/>
    **Lưu ý:** Đường dẫn sổ đăng ký Office 2016 đã thay đổi thành 16.0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Hãy thử quy [trình phục hồi người dùng](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) để khắc phục lỗi Mô-đun Nền tảng Tin cậy (TPM).
- Đặt EnableADAL = 0 theo các bước sau:  
    1. Bấm chuột phải vào Windows Bắt đầu, chọn **Chạy**, nhập **regedit**, sau đó chọn **OK.**
    2. Chọn Có **để cho** phép Trình soạn thảo Sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.
    3. Trong Trình soạn thảo Sổ đăng ký, thêm giá trị DWORD của **EnableADAL** với cài **đặt 0** bên dưới HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Để biết thêm thông tin, hãy xem mục Sự cố kết nối khi đăng nhập sau khi cập [nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)