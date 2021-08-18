---
title: Chặn hoặc bỏ chặn tự động chuyển tiếp email bên ngoài
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897490"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Chặn hoặc bỏ chặn tự động chuyển tiếp email

Để bật hoặc tắt chuyển tiếp email cho một hộp thư cụ thể, hãy xem mục [Đặt cấu hình chuyển tiếp email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Người quản trị có thể kiểm soát chuyển tiếp bên ngoài cho tổ chức bằng cách sử [dụng chính sách thư rác gửi đi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Bạn quản lý chính sách thư rác đi trong cổng thông tin Bộ bảo vệ Microsoft 365 tại hoặc bằng cách sử dụng lệnh ghép ngắn <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) trong Exchange Online PowerShell.

Nếu bạn gặp lỗi sau: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access** bị từ chối, Tổ chức của bạn không cho phép chuyển tiếp bên ngoài", hãy đảm bảo chính sách được đặt cấu hình để bật thư tự động chuyển tiếp bên ngoài.

**Lưu** ý : Chúng tôi đã đề  xuất giá trị mặc định Tự động **-** Hệ thống được kiểm soát cho thiết đặt Quy tắc chuyển tiếp tự động trong chính sách bộ lọc thư rác đi mặc định của bạn (tự động chuyển tiếp bên ngoài bị chặn; tính năng chuyển tiếp tự động nội bộ vẫn hoạt động). Bạn nên tạo chính sách bộ lọc thư rác đi tùy chỉnh và sử dụng giá trị **Bật -** Chuyển tiếp chỉ được kích hoạt cho người dùng cần tự động chuyển tiếp email bên ngoài. Để biết thêm thông tin, [hãy xem mục Đặt cấu hình chuyển tiếp email bên Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
