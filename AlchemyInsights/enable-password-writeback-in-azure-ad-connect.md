---
title: Bật lại mật khẩu trong Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709749"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Bật lại mật khẩu trong Azure AD Connect

Để bật lại bản đặt lại mật khẩu tự phục vụ, trước tiên, bật tùy chọn writeback trong Azure AD Connect. Từ máy chủ Azure AD Connect của bạn, hãy hoàn thành các bước sau đây:

1. Đăng nhập vào máy chủ Azure AD Connect của bạn và bắt đầu trình hướng dẫn cấu hình **AZURE AD Connect** .
2. Trên trang **chào mừng** , bấm **cấu hình**.
3. Trên trang **nhiệm vụ bổ sung** , hãy chọn tùy **chỉnh tùy chọn đồng bộ**, rồi bấm vào **tiếp theo**.
4. Trên trang **kết nối đến AZURE AD** , nhập thông tin xác thực người quản trị toàn cầu cho đối tượng thuê Azure của bạn, rồi bấm vào tiếp theo.
5. Trên trang các **thư mục kết nối** và **tên miền/ou** lọc, bấm **tiếp**.
6. Trên trang **tính năng tùy chọn** , chọn hộp bên cạnh **mật khẩu trở lại** và bấm **tiếp**.
7. Trên trang **sẵn sàng cấu hình** , hãy bấm **cấu hình** và chờ cho quá trình kết thúc.
8. Khi bạn nhìn thấy kết thúc cấu hình, hãy bấm **thoát**.

Với mật khẩu được bật lại trong Azure AD Connect, giờ đây, hãy cấu hình Azure AD SSPR cho writeback.  Để bật lại mật khẩu trong SSPR, hãy hoàn thành các bước sau đây:

1. Đăng nhập vào cổng thông tin Azure bằng tài khoản người quản trị toàn cầu.
2. Tìm kiếm và chọn **Azure Active Directory**, bấm vào **đặt lại mật khẩu**, sau đó chọn **tích hợp tại cơ sở**.
3. Đặt tùy chọn để **ghi lại mật khẩu vào thư mục tại chỗ của bạn?** để **có**.
4. Đặt tùy chọn cho **phép người dùng mở khóa tài khoản mà không đặt lại mật khẩu của họ?** để **có**.
5. Khi đã sẵn sàng, hãy bấm **lưu**.

Để biết thêm thông tin, hãy xem [bật thiết đặt lại mật khẩu tự phục vụ Azure Active Directory với môi trường tại chỗ](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
