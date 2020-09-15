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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695309"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Màn hình đăng nhập trống trong các ứng dụng Microsoft 365

Để khắc phục sự cố này, hãy thử làm như sau:
- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Đặt lại tùy chọn Internet Explorer: đi tới **công cụ**  >  **tùy chọn Internet**  >  **nâng cao**  >  **thiết đặt đặt lại Internet Explorer** (lưu ý rằng bạn sẽ mất thiết đặt tùy chỉnh), rồi thử đăng nhập lại vào Office.
- Tắt bộ bảo vệ ứng dụng Windows Defender (WDAG) hoặc các tường lửa tương tự hoặc chương trình chống vi-rút:
    1. Trong Pa-nen điều khiển, đi tới **chương trình**, rồi chọn **bật hoặc tắt tính năng Windows**.
    2. Nếu bộ bảo vệ ứng dụng Windows Defender được bật, hãy thử tắt tính năng này.<br/>
    **Lưu ý:** Bạn có thể cần phải khởi động lại máy tính.
- Đảm bảo rằng Microsoft...... [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ...........................................
- [Xóa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)

Để biết thêm thông tin, hãy xem các [vấn đề về kết nối trong đăng nhập sau khi cập nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).