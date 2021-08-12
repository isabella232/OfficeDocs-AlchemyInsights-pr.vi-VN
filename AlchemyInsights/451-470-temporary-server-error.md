---
title: 451 4.7.0 Lỗi máy chủ tạm thời. Vui lòng thử lại sau. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812595"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Lỗi máy chủ tạm thời. Vui lòng thử lại sau. PRX4

Bạn có thể gặp phải sự cố trong khi gửi email qua "smtp.office365.com" Smarthost bằng cách sử dụng phương pháp Gửi Máy khách SMTP và nhận được lỗi: "451 4.7.0 Lỗi máy chủ tạm thời. Vui lòng thử lại sau. PRX4 chủ yếu là tạm thời". 

Hãy đảm bảo rằng bạn đang không sử dụng hộp thư chung cho Gửi Máy khách SMTP, vì phương pháp Gửi máy khách SMTP yêu cầu hộp thư được cấp phép để gửi thư thông qua. Tuy nhiên, nếu bạn không sử dụng hộp thư chung và sự cố vẫn tiếp diễn, hãy kiểm tra các mục sau:

1. Bật gửi SMTP máy khách trên hộp thư được cấp phép đang được sử dụng bằng cách chạy lệnh PowerShell này:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    HOẶC

    1. Đi tới danh Trung tâm quản trị Microsoft 365 > **Người dùng hiện hoạt**, rồi chọn người dùng.
    1. Đi tới tab Thư trong > **Dụng email mới** > Quản lý ứng dụng **email**. 
    1. Đảm bảo chọn **thiết đặt SMTP Đã** xác thực (đã bật).
    1. Chọn **Lưu thay đổi**.
    
    Để bật Xác thực SMTP cho toàn bộ tổ chức, hãy chạy lệnh này:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Lưu** ý : Vì lý do bảo mật, bạn nên chỉ bật Xác thực SMTP cho hộp thư đang được sử dụng. Thiết đặt mức người dùng ghi đè lên thiết đặt cấp độ tổ chức.

2. Tắt Mặc định Bảo mật Azure bằng cách chuyển Bật **mặc định bảo mật** thành **Không:**

    1. Đăng nhập vào cổng thông tin Azure với tư cách người quản trị bảo mật, người quản trị Truy nhập có Điều kiện hoặc người quản trị toàn cầu.
    1. Duyệt đến Thuộc Azure Active Directory >**  tính ,** rồi chọn Quản **lý mặc định bảo mật**.
    1. Đặt nút **bật tắt Bật mặc định** bảo mật thành **Không.**
    1. Chọn **Lưu**.

3. Tắt Xác thực Đa Yếu tố (MFA) trên hộp thư được cấp phép đang được sử dụng.

    1. Đi tới menu Trung tâm quản trị Microsoft 365, rồi trong menu dẫn hướng bên trái, chọn Người dùng **người dùng**  >  **hiện hoạt.**
    1. Trên trang **Người dùng hiện** hoạt, chọn Xác thực đa yếu **tố**.
    1. Chọn người dùng, rồi tắt **Xác thực đa yếu tố.**

