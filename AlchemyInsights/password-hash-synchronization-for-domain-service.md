---
title: Đồng bộ hóa băm mật khẩu cho dịch vụ tên miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040888"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Đồng bộ hóa băm mật khẩu cho dịch vụ tên miền

**Nếu phiên bản Azure AD DS của bạn nhắc bạn bật đồng bộ hóa băm mật khẩu**

Bạn gặp phải kịch bản trong đó bạn đang chạy môi trường kết hợp với người dùng đồng bộ hóa từ môi trường Dịch vụ Miền Azure Active Directory tại chỗ (AD DS). Bạn vẫn gặp phải kịch bản này mặc dù bạn có đồng bộ hóa băm mật khẩu từ AD DS tại chỗ với đối tượng thuê Azure AD của mình.

**Nguyên nhân**

Điều này xảy ra vì Azure AD Kết nối theo mặc định không đồng bộ hóa Thừa tự Trình quản lý Công nghệ LAN (NTLM) và hashe mật khẩu Kerberos cần thiết cho Azure AD DS.

**Giải pháp thay thế** 

You would need to configure Azure AD Kết nối to synchronize those password hashes required for NTLM and Kerberos authentication.

Sau khi Azure AD Kết nối cấu hình, sự kiện tạo tài khoản hoặc thay đổi mật khẩu tại chỗ cũng sẽ đồng bộ hóa các hashe mật khẩu thừa tự với Azure AD. Vui lòng xem [tại](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) đây để biết thêm thông tin về điều này và để biết hướng dẫn về cách bật đồng bộ hóa mật khẩu trong môi trường kết hợp Azure AD DS.