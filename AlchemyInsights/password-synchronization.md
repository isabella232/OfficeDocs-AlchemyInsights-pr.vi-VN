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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483089"
---
# <a name="password-synchronization"></a>Đồng bộ hoá mật khẩu

**Đồng bộ hóa hash mật khẩu không hoạt động ở tất cả**

Một số khách hàng thường gặp sự cố khi đồng bộ hóa hash mật khẩu không hoạt động là:

- Tài khoản Active Directory được sử dụng bởi Azure AD Connect để liên lạc với Active Directory tại chỗ không được cấp cho các **thay đổi thư mục** nhân bản và nhân rộng **thay đổi tất cả** các quyền, vốn cần thiết cho việc đồng bộ hóa mật khẩu-bạn cần phải khắc phục sự cố này bằng cách cấp các quyền đối với tài khoản Active Directory.
- Đồng bộ hóa hash mật khẩu bị vô hiệu hóa sau khi người quản trị thay đổi phương pháp Sign-In người dùng từ việc **đồng bộ hóa mật khẩu** đến một tùy chọn khác chẳng hạn như **liên kết với AD FS** trong trình hướng dẫn kết nối Azure AD-bạn có thể khắc phục điều này bằng cách bật lại tính năng **đồng bộ hóa hash mật khẩu** trong trình hướng dẫn Azure AD Connect.
- Vấn đề kết nối với Active Directory tại chỗ. Ví dụ: một số bộ điều khiển tên miền không được truy nhập bằng Azure AD Connect, hoặc các [cổng bắt buộc](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) bị tường lửa-bạn cần khắc phục điều này bằng cách đảm bảo rằng kết nối giữa máy chủ Azure AD Connect và Active Directory tại chỗ hoạt động chính xác.
- Máy chủ Azure AD Connect hiện đang ở chế độ tổ chức, vốn sẽ kết quả là máy chủ không thể sử dụng để khắc phục sự cố này, hãy làm theo các bước được mô tả trong phần [khắc phục sự cố mật khẩu đồng bộ hóa với AZURE AD Connect Sync-không có mật khẩu được đồng bộ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Đồng bộ hóa hash mật khẩu không hoạt động đối với một số người dùng của tôi**

1. Nếu bạn nhận thấy rằng băm mật khẩu không đồng bộ với người dùng, hãy sử dụng tác vụ **khắc phục sự cố** trong Azure AD Connect để điều tra và giải quyết sự cố. Thực hiện các tác vụ sau đây:

    một. [Chạy nhiệm vụ khắc phục sự cố trong trình hướng dẫn](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Sử dụng lệnh ghép ngắn khắc phục sự cố để điều tra sự cố đồng bộ hóa mật khẩu của Hash cho một dùng cụ thể](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Đối tượng người dùng Active Directory tại chỗ được kích hoạt cho **người dùng phải thay đổi mật khẩu tại tùy chọn đăng nhập tiếp theo** . Khi tùy chọn này được bật, người dùng được gán một mật khẩu tạm thời và sẽ được nhắc thay đổi mật khẩu trong đăng nhập tiếp theo. Azure AD Connect sẽ không đồng bộ hóa mật khẩu tạm thời cho Azure AD.

Để giải quyết sự cố trên đây, hãy thực hiện một trong các tác vụ sau:

- Yêu cầu người dùng đăng nhập vào ứng dụng tại cơ sở (ví dụ, Windows Desktop) và thay đổi mật khẩu. Mật khẩu mới sẽ được đồng bộ hóa với Azure AD.
- Có người quản trị Cập nhật mật khẩu của người dùng mà không cho phép **người dùng tùy chọn phải thay đổi mật khẩu tại mục đăng nhập tiếp theo** và chia sẻ mật khẩu mới với người dùng.

3. Đối tượng người dùng Active Directory tại cơ sở **không được cấu hình chính xác** cho đồng bộ hóa đối tượng hoặc đồng bộ hóa mật khẩu. Để khắc phục sự cố này, hãy làm theo các bước được mô tả trong [đồng bộ hóa hash mật khẩu khắc phục sự cố với AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







