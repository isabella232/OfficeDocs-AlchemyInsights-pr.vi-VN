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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579923"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Màn hình đăng nhập trống trong ứng dụng Microsoft 365

Để khắc phục sự cố này, hãy thử như sau:
- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Đặt lại tùy chọn Internet Explorer: đi tới **công cụ**  >  **tùy chọn Internet**  >  **nâng cao**thiết lập  >  **lại Internet Explorer cài đặt** (lưu ý rằng bạn sẽ mất cài đặt tuỳ chỉnh), và sau đó thử đăng nhập vào Office một lần nữa.
- Vô hiệu hoá Windows Defender Application guard (WDAG) hoặc bất kỳ tường lửa tương tự hoặc chương trình chống vi-rút:
    1. Trong Pa-nen điều khiển, đi tới **chương trình**, sau đó chọn **bật hoặc tắt tính năng của Windows**.
    2. Nếu bộ bảo vệ ứng dụng Windows Defender được bật, hãy thử tắt.<br/>
    **Lưu ý:** Bạn có thể phải khởi động lại máy tính.
- Đảm bảo rằng Microsoft. AAD. BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) không bị chặn bởi bất kỳ ứng dụng hoặc tường lửa/chương trình chống vi-rút.
- [Thông tin đăng nhập văn phòng rõ ràng](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm Windows.<br/>
    **Lưu ý:** Đường dẫn đăng ký cho Office 2016 đã thay đổi để 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)

Để biết thêm thông tin, [hãy xem sự cố kết nối trong đăng nhập sau khi Cập Nhật cho Office 2016 xây dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).