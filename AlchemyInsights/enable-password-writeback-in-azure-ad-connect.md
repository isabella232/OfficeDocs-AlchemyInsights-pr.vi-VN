---
title: Bật ghi lại mật khẩu trong Azure AD Kết nối
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325409"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Bật ghi lại mật khẩu trong Azure AD Kết nối

Để bật chức năng ghi lại mật khẩu tự phục vụ, trước tiên hãy bật tùy chọn ghi lại trong Azure AD Kết nối. Từ máy chủ Azure AD Kết nối của bạn, hãy hoàn tất các bước sau đây:

1. Đăng nhập vào máy chủ Azure AD Kết nối khởi động trình hướng **dẫn cấu hình Azure AD Kết nối** hình.
2. Trên trang Chào **mừng,** bấm **Cấu hình.**
3. Trên trang **Tác vụ bổ** sung, chọn Tùy chỉnh tùy chọn **đồng** bộ hóa , rồi bấm vào **Tiếp theo.**
4. Trên trang **Kết nối Azure AD,** nhập thông tin xác thực người quản trị toàn cầu cho đối tượng thuê Azure của bạn, rồi bấm vào **Tiếp theo**.
5. Trên các **Kết nối mục và trang** lọc Tên **miền/OU,** bấm vào **Tiếp theo.**
6. Trên trang **Tính năng tùy** chọn, chọn hộp bên cạnh Ghi lại mật **khẩu, rồi** bấm vào Tiếp **theo.**
7. Trên trang **Sẵn sàng cấu hình,** hãy bấm **Cấu** hình và đợi cho đến khi kết thúc quy trình.
8. Khi bạn thấy cấu hình hoàn tất, hãy bấm **Thoát.**

Với chức năng ghi lại mật khẩu được bật trong Azure AD Kết nối, hãy đặt cấu hình Azure AD SSPR để ghi lại.  Để bật ghi lại mật khẩu trong SSPR, hãy hoàn thành các bước sau đây:

1. Đăng nhập vào cổng thông tin Azure bằng tài khoản người quản trị toàn cầu.
2. Tìm kiếm và chọn cài **Azure Active Directory**, bấm **đặt lại mật** khẩu , sau đó bấm tích hợp tại **chỗ**.
3. Đặt tùy chọn Ghi **lại mật khẩu vào thư mục tại chỗ của bạn?** thành **Có**.
4. Đặt tùy chọn Cho phép **người dùng mở khóa tài khoản mà không đặt lại mật khẩu?** **thành Có.**
5. Khi đã sẵn sàng, hãy **bấm Lưu**.

Để biết thêm thông tin, hãy xem Azure Active Directory bật tính năng tự đặt lại mật khẩu [ghi lại về môi trường tại chỗ.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

**Lưu** ý: Khi người quản trị đặt lại mật khẩu người dùng trong Cổng thông tin Azure, nếu người dùng đó được liên kết hoặc đồng bộ hóa mật khẩu, mật khẩu sẽ được ghi trở lại mật khẩu tại chỗ. Chức năng này yêu cầu Giấy Premium Azure (P1 hoặc P2) và hiện không được hỗ trợ trong cổng thông tin Quản Office của bạn.
