---
title: Đồng bộ hóa hash mật khẩu cho dịch vụ miền
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
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177616"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Đồng bộ hóa hash mật khẩu cho dịch vụ miền

**Nếu ví dụ Azure AD DS của bạn là nhắc bạn bật đồng bộ hóa hash mật khẩu**

Bạn gặp phải một tình huống mà bạn đang chạy môi trường hỗn hợp với người dùng đang đồng bộ hóa từ môi trường dịch vụ miền (AD DS) tại chỗ của Azure Active Directory. Tình huống này gặp mặc dù bạn có đồng bộ hóa hash mật khẩu từ AD DS tại cơ sở với đối tượng thuê Azure AD của bạn.

**Bởi**

Điều này xảy ra vì Azure AD kết nối theo mặc định không đồng bộ hóa công nghệ mới của Microsoft Manager (NTLM) và Kerberos mật khẩu hàm băm cần thiết cho Azure AD DS.

**Lỗi** 

Bạn sẽ cần phải cấu hình Azure AD Connect để đồng bộ hóa các hàm hàm băm mật khẩu được yêu cầu cho NTLM và Kerberos xác thực.

Sau khi Azure AD Connect được cấu hình, một tài khoản tại chỗ hoặc tạo sự kiện thay đổi mật khẩu cũng đồng bộ hóa mật khẩu kế thừa hàm băm thành Azure AD. Vui lòng xem mục [ở đây](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) để biết thêm thông tin về điều này và để được hướng dẫn về cách bật đồng bộ hóa mật khẩu trong AZURE AD DS Hybrid môi trường.