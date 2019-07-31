---
title: Vấn đề đăng nhập vào ứng dụng văn phòng
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938391"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Đăng nhập màn hình trống trong các ứng dụng văn phòng

Để khắc phục vấn đề này, hãy thử như sau:
- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Đặt lại tuỳ chọn Internet Explorer: vào **Tools** > **Internet Options** > **cao** > **Reset Internet Explorer Settings** (lưu ý rằng bạn sẽ mất các thiết đặt tùy chỉnh), và sau đó cố gắng đăng nhập vào văn phòng một lần nữa.
- Vô hiệu hóa Windows Defender áp dụng Guard (WDAG) hoặc bất kỳ chương trình tương tự như tường lửa hoặc chống vi-rút:
    1. Trong bảng điều khiển, đi đến **các chương trình**, và sau đó chọn **Turn Windows features Baät hoaëc taét**.
    2. Nếu bảo vệ ứng dụng Windows Defender được bật, hãy thử vô hiệu hóa nó.<br/>
    **Lưu ý:** Bạn có thể cần phải khởi động lại máy tính.
- Đảm bảo rằng Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) không bị chặn bởi bất kỳ ứng dụng hoặc tường lửa/chống-virus chương trình.
- [Rõ ràng văn phòng thông tin đăng nhập](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) bằng cách sử dụng trình quản lý ủy nhiệm của Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký đối với Office 2016 đã thay đổi để 16.0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)

Để biết thêm chi tiết, hãy xem [kết nối các vấn đề trong đăng nhập sau khi Cập Nhật cho Office 2016 build 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).