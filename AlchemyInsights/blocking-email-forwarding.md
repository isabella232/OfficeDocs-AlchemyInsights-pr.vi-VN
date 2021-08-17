---
title: 726 Chặn chuyển tiếp email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059654"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Chặn hoặc bỏ chặn chuyển tiếp email

Để bật hoặc tắt chuyển tiếp email cho một hộp thư cụ thể, hãy xem mục [Đặt cấu hình chuyển tiếp email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Ở cấp độ đối tượng thuê, việc kiểm soát chuyển tiếp bên ngoài được thực hiện bằng cách sử dụng chính sách thư rác đi. Bạn có thể kiểm tra chính sách [](https://protection.office.com/antispam) bộ lọc thư rác đi từ Trung tâm Bảo mật và Tuân thủ tại đây hoặc bằng cách sử dụng lệnh [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Nếu bạn gặp lỗi sau: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access** bị từ chối, Tổ chức của bạn không cho phép chuyển tiếp bên ngoài", vui lòng đảm bảo chính sách được đặt cấu hình để bật tự động chuyển tiếp bên ngoài.

**Lưu ý:** Chúng tôi khuyên bạn nên tắt Tự động Gửi đi bên ngoài trên chính sách bộ lọc thư rác gửi đi mặc định của bạn và chỉ bật tính năng này cho những người dùng cần chuyển tiếp bên ngoài bằng cách tạo một chính sách tùy chỉnh cho những người dùng đó. Bạn có thể đọc thêm trong [phần Đặt cấu hình chuyển tiếp email bên Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)