---
title: Thu hồi hoặc thay thế thư email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024408"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Thu hồi hoặc thay thế thư email trong Microsoft 365

- Bạn chỉ có **thể thu hồi thư được gửi đến những người trong tổ chức của bạn.** Ví dụ, nếu thư đã được gửi đến một địa chỉ Gmail, bạn không thể thu hồi thư.
- Bạn chỉ **có thể thu hồi thư đã gửi Outlook gửi cho PC**. Nếu người dùng gửi thư bằng Outlook for Mac hoặc Outlook trên web thì bạn không thể thu hồi thư.
- Là người quản trị đối tượng thuê, bạn có thể thu hồi thư thay mặt người dùng bằng cách sử dụng **PowerShell** (Để biết thêm thông tin, hãy xem: Tìm kiếm [và xóa thư email).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Bạn không thể thu hồi thư từ trung tâm quản trị. Cuộn xuống đến "Tìm kiếm và xóa thư email trong tổ chức của bạn" để biết thêm thông tin.

**Thu hồi hoặc thay thế thư email mà bạn đã gửi**

1. Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục Mục đã gửi.
2. Mở thư bạn muốn thu hồi. Bạn phải bấm đúp để mở thư. Việc chọn thư để hiển thị trong ngăn đọc sẽ không cho phép bạn thu hồi thư.
3. Từ tab Thư, chọn Hành động **Thu hồi**  >  **Thư Này**.
4. Chọn **Xóa bản sao chưa đọc của thư này hoặc** Xóa bản sao chưa đọc và thay thế bằng thư **mới**, sau đó chọn **OK.**
5. Nếu bạn đang gửi thư thay thế, hãy soạn thư, sau đó chọn **Gửi**.
6. Sự thành công hoặc thất bại của việc thu hồi thư phụ thuộc vào thiết đặt của người nhận trong Outlook.

Để biết thêm thông tin, bao gồm cách kiểm tra việc thu hồi, hãy xem [Thu hồi hoặc thay thế thư email mà bạn đã gửi](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Để tìm kiếm và xóa thư email trong tổ chức của bạn***, đây là cách dễ nhất nếu bạn là người quản trị toàn cầu. Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào nhóm vai trò Trình quản lý Khám phá Điện tử hoặc vào vai trò quản lý Tìm kiếm Tuân thủ. Để xóa thư, bạn sẽ cần tham gia nhóm vai trò Quản lý Tổ chức hoặc vai trò quản lý Tìm kiếm và Dọn sạch. Quyền đối với các vai trò này được gán trong [Trung tâm Bảo & tuân thủ.](https://protection.office.com/)

1. [Tạo một tìm kiếm nội](https://docs.microsoft.com/microsoft-365/compliance/content-search) dung để tìm thư cần xóa.
2. [Kết nối tâm Bảo mật & Tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Nếu bạn đang sử dụng MFA (xác thực đa yếu tố), hãy xem Kết nối để Microsoft 365 Trung tâm Bảo mật & Tuân thủ [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)bằng xác thực đa yếu tố.
