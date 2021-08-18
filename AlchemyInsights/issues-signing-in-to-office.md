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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088058"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Màn hình đăng nhập trống trong ứng Microsoft 365 dụng

Để khắc phục sự cố này, hãy thử làm như sau:
- Cài đặt các bản cập nhật mới [nhất cho Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Đặt lại tùy chọn Internet Explorer: Đi đến Công cụ Tùy chọn Internet Nâng cao Đặt lại  >    >    >  **Internet Explorer Cài đặt** (lưu ý rằng bạn sẽ mất các thiết đặt tùy chỉnh), rồi thử đăng nhập lại Office.
- Vô hiệu hóa trình Tính năng Bảo vệ Ứng dụng của Bộ bảo vệ Windows (WDAG) hoặc bất kỳ tường lửa hoặc chương trình chống vi rút tương tự nào:
    1. Trong Panel Điều khiển, đi **tới Chương** trình , rồi chọn Bật Windows **năng mới**.
    2. Nếu Tính năng Bảo vệ Ứng dụng của Bộ bảo vệ Windows được bật, hãy thử tắt nó.<br/>
    **Lưu ý:** Bạn có thể cần khởi động lại máy tính.
- Đảm bảo rằng chương trình bổ trợ Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) không bị bất kỳ ứng dụng hoặc chương trình tường lửa/chương trình chống vi rút nào chặn.
- [Xóa thông Office tin xác thực](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách Windows Trình quản lý chứng danh.<br/>
    **Lưu ý:** Đường dẫn sổ đăng ký Office 2016 đã thay đổi thành 16.0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)

Để biết thêm thông tin, hãy xem mục Sự cố kết nối khi đăng nhập sau khi cập [nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)