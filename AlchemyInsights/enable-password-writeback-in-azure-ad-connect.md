---
title: Bật ghi lại mật khẩu trong Azure AD kết nối
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204646"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Bật ghi lại mật khẩu trong Azure AD kết nối

Để bật lại ghi lại mật khẩu tự dịch vụ, trước tiên cho phép tuỳ chọn quay lại trong Azure AD kết nối. Từ máy chủ Azure AD kết nối, hoàn thành các bước sau:

1. Đăng nhập vào máy chủ Azure AD kết nối của bạn và khởi động thuật sĩ cấu hình **AZURE AD kết nối** .
2. Trên trang **chào mừng** , bấm **cấu hình**.
3. Trang **tác vụ bổ sung** , chọn **tuỳ chỉnh tùy chọn đồng bộ hóa**, và sau đó nhấp vào **tiếp theo**.
4. Trên trang **kết nối AZURE AD** , nhập uỷ nhiệm quản trị viên chung cho thuê Azure của bạn, và sau đó nhấp vào tiếp theo.
5. Trên các **thư mục kết nối** và **miền/ou** lọc trang, bấm vào **tiếp theo**.
6. Trên trang **tính năng tùy chọn** , chọn hộp bên cạnh ghi **lại mật khẩu** và nhấp vào **tiếp theo**.
7. Trên **sẵn sàng để cấu hình** trang, bấm **cấu hình** và chờ cho quá trình kết thúc.
8. Khi bạn thấy kết thúc cấu hình, bấm **thoát**.

Với ghi lại mật khẩu được kích hoạt trong Azure AD kết nối, bây giờ cấu hình Azure AD SSPR để ghi lại.  Để kích hoạt ghi lại mật khẩu trong SSPR, hoàn thành các bước sau:

1. Đăng nhập vào cổng thông tin Azure bằng tài khoản quản trị viên chung.
2. Tìm kiếm và chọn **Azure Active Directory**, bấm **đặt lại mật khẩu**, sau đó chọn **tích hợp tại chỗ**.
3. Đặt tùy chọn **để ghi lại mật khẩu vào thư mục tại chỗ của bạn?** để **có**.
4. Thiết lập tùy chọn cho **phép người dùng mở khóa tài khoản mà không đặt lại mật khẩu của họ?** để **có**.
5. Khi đã sẵn sàng, hãy nhấp vào **lưu**.

Để biết thêm thông tin, xem [bật lại mật khẩu Azure Active Directory tự dịch vụ ghi ghi lại vào môi trường tại chỗ](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
