---
title: 726 chặn chuyển tiếp email
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478336"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Chặn hoặc bỏ chặn chuyển tiếp email

Để bật hoặc tắt tính năng chuyển tiếp email cho một hộp thư cụ thể, hãy xem mục [đặt cấu hình chuyển tiếp email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Trên mức đối tượng thuê, kiểm soát việc chuyển tiếp bên ngoài được thực hiện bằng cách sử dụng chính sách thư rác đi. Bạn có thể kiểm tra chính sách lọc thư rác từ Trung tâm bảo mật và tuân thủ [tại đây](https://protection.office.com/antispam) hoặc bằng cách sử dụng [lệnh Get-Hostenhoutboundspamfilterpolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Nếu bạn nhận được lỗi sau: **"550 5.7.520 Access bị từ chối, tổ chức của bạn không cho phép chuyển tiếp bên ngoài"**, hãy đảm bảo rằng chính sách được cấu hình để cho phép tự động chuyển tiếp bên ngoài.

**Lưu ý:** Khuyên bạn nên giữ tự động tắt tiếng ở bên ngoài trong chính sách bộ lọc thư rác mặc định của bạn và bật tính năng này chỉ dành cho những người dùng cần chuyển tiếp bên ngoài bằng cách tạo chính sách tùy chỉnh cho những người dùng đó. Bạn có thể đọc thêm trong [cấu hình chuyển tiếp email bên ngoài trong Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).