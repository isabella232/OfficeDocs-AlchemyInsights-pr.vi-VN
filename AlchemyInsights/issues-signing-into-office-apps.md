---
title: Sự cố khi đăng nhập vào ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579887"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Khắc phục các ứng dụng Microsoft 365 "mô-đun nền tảng đáng tin cậy của máy tính không hoạt động đúng" thông báo

Để khắc phục lỗi này, hãy thử như sau:

- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.<br/>
    **Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Hãy thử [quá trình khôi phục người dùng](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) để khắc phục lỗi nền tảng đáng tin cậy (TPM).
- Đặt EnableADAL = 0 bằng cách sử dụng các bước sau:  
    1. Bấm chuột phải vào nút khởi động Windows, chọn **chạy**, gõ **regedit**, và sau đó chọn **OK**.
    2. Chọn **có** để cho phép Registry Editor thực hiện thay đổi cho thiết bị của bạn.
    3. Trong Registry Editor, thêm một giá trị của **Enableadal** với một thiết lập **0** trong HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Để biết thêm thông tin, [hãy xem sự cố kết nối trong đăng nhập sau khi Cập Nhật cho Office 2016 xây dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).