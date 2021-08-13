---
title: Đồng bộ hoá mật khẩu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960857"
---
# <a name="password-synchronization"></a>Đồng bộ hoá mật khẩu

**Đồng bộ hóa Băm Mật khẩu hoàn toàn không hoạt động**

Một số sự cố phổ biến mà khách hàng gặp phải khi Đồng bộ hóa Băm Mật khẩu không hoạt động:

- Tài khoản Active Directory được Azure AD Kết nối sử dụng để liên lạc  với Active  Directory tại chỗ sẽ không được cấp Sao chép Thay đổi Thư mục và Nhân bản Thay đổi Thư mục Tất cả những quyền cần thiết để đồng bộ hóa mật khẩu - Bạn cần khắc phục sự cố này bằng cách cấp các quyền này cho tài khoản Active Directory.
- Tính năng đồng bộ hóa băm mật khẩu sẽ bị  tắt sau khi người quản trị thay đổi phương pháp Sign-In Người dùng từ Đồng bộ  hóa Mật khẩu sang một tùy chọn khác, như Liên kết với **AD FS** trong trình hướng dẫn Azure AD Kết nối - Bạn có thể khắc phục sự cố này bằng cách bật lại tính năng đồng bộ hóa băm mật khẩu trong trình hướng dẫn Azure AD Kết nối.
- Vấn đề về kết nối với Active Directory tại cơ sở. Ví dụ: một số bộ kiểm soát miền không thể [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) truy nhập bằng Azure AD Kết nối hoặc Tường lửa yêu cầu chặn một số cổng - Bạn cần khắc phục điều này bằng cách đảm bảo rằng kết nối giữa máy chủ Azure AD Kết nối và Active Directory tại chỗ hoạt động đúng cách.
- Máy chủ Azure AD Kết nối hiện đang ở chế độ cá nhân hóa, điều này sẽ khiến máy chủ không thể nhập các băm mật khẩu - Để khắc phục sự cố, hãy làm theo các bước được mô tả trong mục Khắc phục sự cố đồng bộ hóa mật khẩu với đồng bộ [Azure AD Kết nối -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Không mật khẩu nào được đồng bộ.

**Đồng bộ hóa Băm Mật khẩu không hoạt động đối với một số người dùng của tôi**

1. Nếu bạn nhận thấy rằng băm mật khẩu không  đồng bộ hóa với người dùng, hãy sử dụng tác vụ khắc phục sự cố trong Azure AD Kết nối để điều tra và giải quyết sự cố. Thực hiện các tác vụ sau:

    a. [Chạy nhiệm vụ khắc phục sự cố trong trình hướng dẫn](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Sử dụng lệnh ghép ngắn khắc phục sự cố để điều tra sự cố đồng bộ hóa băm mật khẩu cho một mục đích sử dụng cụ thể](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Đối tượng Người dùng Active Directory tại cơ sở được bật cho Người dùng phải **thay đổi mật khẩu ở tùy chọn đăng nhập tiếp** theo. Khi tùy chọn này được bật, người dùng sẽ được gán một mật khẩu tạm thời và sẽ được nhắc thay đổi mật khẩu trên lần đăng nhập tiếp theo. Azure AD Kết nối đồng bộ hóa mật khẩu tạm thời với Azure AD.

Để giải quyết vấn đề trên, hãy thực hiện một trong các tác vụ sau đây:

- Yêu cầu người dùng đăng nhập vào ứng dụng tại chỗ (ví dụ: màn Windows máy tính) và thay đổi mật khẩu. Mật khẩu mới sẽ được đồng bộ hóa với Azure AD.
- Hãy để người quản trị cập nhật mật khẩu của người dùng mà không bật tùy chọn Người dùng phải thay đổi mật khẩu ở lần đăng nhập tiếp theo **và** chia sẻ mật khẩu mới với người dùng.

3. Đối tượng Người dùng Active  Directory tại chỗ không được đặt cấu hình chính xác để đồng bộ hóa đối tượng hoặc đồng bộ hóa mật khẩu. Để khắc phục sự cố này, hãy làm theo các bước được mô tả trong mục Khắc phục sự cố đồng bộ hóa băm mật khẩu [với Azure AD Kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







