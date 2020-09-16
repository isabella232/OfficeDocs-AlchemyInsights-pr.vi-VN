---
title: Đăng nhập vào Windows 10 mà không cần dùng mật khẩu
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719975"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Đăng nhập vào Windows 10 mà không cần dùng mật khẩu

Để tránh việc nhập mật khẩu tại khởi động Windows, chúng tôi khuyên bạn nên sử dụng một trong các tùy chọn đăng nhập bảo mật của Windows hello, chẳng hạn như mã PIN, nhận diện khuôn mặt hoặc dấu vân tay, nếu có. Nếu bạn thực sự muốn tắt tính năng đăng nhập bảo mật, hãy xem hướng dẫn "tự động đăng nhập vào Windows 10" bên dưới.

**Bảo mật cho các lựa chọn thay thế Windows hello vào mật khẩu tài khoản**

Đi đến **cài đặt > tài khoản > các tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)). Các tùy chọn đăng nhập sẵn dùng sẽ được liệt kê. Ví dụ:

![Các tùy chọn đăng nhập.](media/sign-in-options.png)

Bấm hoặc gõ nhẹ vào một trong các tùy chọn để cấu hình. Lần sau khi bạn khởi động hoặc mở khóa Windows, bạn sẽ có thể sử dụng tùy chọn mới thay vì mật khẩu. 

**Đăng nhập tự động vào Windows 10**

**Lưu ý**: việc đăng nhập tự động thuận tiện, nhưng giới thiệu một rủi ro bảo mật, đặc biệt là nếu PC của bạn có thể truy nhập được nhiều người. 

1. Bấm hoặc gõ nhẹ vào nút **bắt đầu** trong thanh tác vụ.

2. Nhập **netplwiz** và nhấn phím Enter để mở cửa sổ tài khoản người dùng.

3. Trong **tài khoản người dùng**, hãy bấm vào tài khoản mà bạn muốn tự động đăng nhập vào khi Windows khởi động.

4. Bỏ chọn hộp kiểm "người dùng phải nhập tên người dùng và mật khẩu để dùng hộp kiểm" máy tính này.

    ![Người dùng phải nhập tùy chọn tên người dùng và mật khẩu.](media/users-must-enter-username.png)

5. Bấm **OK**. Bạn sẽ được yêu cầu nhập và xác nhận mật khẩu cho tài khoản mà bạn đã chọn. Bấm vào **OK** để kết thúc. Thời gian tiếp theo, Windows 10 bắt đầu, nó sẽ tự động đăng nhập vào tài khoản mà bạn đã chọn.
