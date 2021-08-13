---
title: Outlook Thu hồi hoặc thay thế thư email trên màn hình nền
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918417"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Thu hồi hoặc thay thế Outlook email

- Với tư cách là người quản trị, **bạn có thể thu hồi thư thay mặt người dùng bằng cách sử dụng PowerShell.** Bạn không thể thu hồi thư từ trung tâm quản trị.
- Bạn chỉ có **thể thu hồi thư được gửi đến những người trong tổ chức của bạn.** Ví dụ, nếu thư đã được gửi đến một địa chỉ Gmail, bạn không thể thu hồi thư.
- Bạn chỉ **có thể thu hồi thư đã gửi Outlook 2016 trên PC .** Nếu người dùng gửi thư bằng Outlook for Mac hoặc Outlook trên web thì bạn không thể thu hồi thư.

Để thu hồi hoặc thay thế thư email:

1. Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục Mục đã gửi.
1. Bấm đúp vào thư bạn muốn thu hồi để mở thư.
1. Chọn tab **Thư,** rồi chọn Hành động **Thu**  >  **hồi Thư Này**.
1. Chọn **Xóa bản sao chưa đọc của thư này hoặc** Xóa bản sao chưa đọc và thay thế **bằng** thư mới , sau đó chọn **OK.**
1. Nếu bạn đang gửi thư thay thế, hãy soạn thư và chọn **Gửi**.
1. Sự thành công hoặc thất bại của việc thu hồi thư phụ thuộc vào thiết đặt của người nhận trong Outlook. Để biết các bước kiểm tra việc thu hồi, hãy xem [bài viết này.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Tìm kiếm và xóa thư email trong tổ chức của bạn

- Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào vai trò Trình quản lý Khám phá Điện tử hoặc vai trò quản lý Tìm kiếm Tuân thủ để tìm kiếm thư. Để xóa thư, bạn sẽ cần tham gia nhóm vai trò Quản lý Tổ chức hoặc vai trò quản lý Tìm kiếm và Dọn sạch. Quyền đối với các vai trò này được gán trong Trung [tâm bảo mật và tuân thủ](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Tạo một tìm kiếm nội](https://docs.microsoft.com/microsoft-365/compliance/content-search) dung để tìm thư cần xóa.
- [Kết nối tâm Bảo mật và Tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Nếu bạn đang sử dụng xác thực đa yếu tố, hãy xem Kết nối để Microsoft 365 tâm bảo mật và tuân thủ [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bằng cách sử dụng xác thực đa yếu tố.