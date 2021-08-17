---
title: Bật xác thực và khắc phục sự cố SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890456"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Bật xác thực và khắc phục sự cố SMTP

Nếu bạn muốn bật xác thực SMTP cho một hộp thư hoặc bạn đang nhận được một "Máy khách chưa được xác thực", Lỗi "Xác thực không thành công" hoặc lỗi "SmtpClientAuthentication" với mã 5.7.57 hoặc 5.7.3 hoặc 5.7.139 khi bạn cố gắng chuyển tiếp email bằng cách xác thực một thiết bị hoặc ứng dụng với Microsoft 365, hãy thực hiện ba hành động này để giải quyết vấn đề này:

1. Tắt mặc [định bảo mật Azure bằng](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) cách chuyển Bật mặc định bảo **mật** thành **Không.**

    a. Đăng nhập vào cổng thông tin Azure với tư cách người quản trị Bảo mật, người quản trị Truy nhập có Điều kiện hoặc người quản trị toàn cầu.<BR/>
    b. Duyệt đến Thuộc Azure Active Directory > **tính**.<BR/>
    c. Chọn **Quản lý mặc định bảo mật**.<BR/>
    d. Đặt **Bật mặc định bảo mật** là **Không**.<BR/>
    e. Chọn **Lưu**.

2. [Bật gửi SMTP máy khách trên](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) hộp thư được cấp phép.

    a. Từ hộp Trung tâm quản trị Microsoft 365, đi tới **Người dùng Hiện hoạt**, rồi chọn người dùng.<BR/>
    b. Đi tới tab Thư và trong Ứng dụng **email**, chọn Quản **lý ứng dụng email**.<BR/>
    d. Đảm bảo đã chọn (đã bật xác thực **SMTP).**<BR/>
    e. Chọn **Lưu thay đổi**.<BR/>

3. [Tắt Xác thực Đa Yếu tố (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) trên hộp thư được cấp phép.

    a. Đi tới menu Trung tâm quản trị Microsoft 365, rồi trong menu dẫn hướng bên trái, chọn Người dùng **Người dùng**  >  **hiện hoạt**.<BR/>
    b. Chọn **Xác thực đa yếu tố**.<BR/>
    c. Chọn người dùng, rồi tắt **xác thực Đa Yếu tố**.<BR/>
