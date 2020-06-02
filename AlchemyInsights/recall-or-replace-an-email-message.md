---
title: Gọi lại hoặc thay thế thư email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509478"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Gọi lại hoặc thay thế thư email trong Microsoft 365

- Bạn chỉ có thể **gọi lại thư được gửi cho những người trong tổ chức của bạn**. Ví dụ: nếu thư được gửi đến địa chỉ Gmail, bạn không thể gọi lại thông báo đó.
- Bạn chỉ có thể **gọi lại thư được gửi từ Outlook 2016 cho máy tính**. Nếu người dùng gửi thư bằng cách sử dụng Outlook dành cho Mac hoặc Outlook trên web, bạn không thể gọi lại.
- Nếu bạn là quản trị viên, bạn có thể **gọi lại thư thay mặt người dùng bằng cách sử dụng PowerShell**. Bạn không thể gọi lại thư từ Trung tâm quản trị. Cuộn xuống mục "tìm kiếm và xóa thư email trong tổ chức của bạn" để biết thêm thông tin.

**Gọi lại hoặc thay thế thư email bạn đã gửi**

1. Trong ngăn thư mục bên trái cửa sổ Outlook, chọn thư mục mục đã gửi.
2. Mở thư mà bạn muốn gọi lại. Bạn phải bấm đúp để mở thư. Chọn thư để nó xuất hiện trong ngăn đọc sẽ không cho phép bạn nhớ lại thư.
3. Từ tab thông điệp, chọn **hành động**  >  **nhớ lại thư này**.
4. Chọn **xóa các bản sao chưa đọc của thư này** hoặc **xóa các bản sao chưa đọc và thay thế bằng một tin nhắn mới**, sau đó chọn **OK**.
5. Nếu bạn đang gửi một tin nhắn thay thế, soạn tin nhắn, sau đó chọn **gửi**.
6. Sự thành công hay thất bại của một tin nhắn thu hồi phụ thuộc vào cài đặt của người nhận trong Outlook.

Để biết thêm thông tin, bao gồm cách kiểm tra thu hồi, hãy xem [gọi lại hoặc thay thế thư email bạn đã gửi](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Tìm kiếm và xóa thư email trong tổ chức của bạn*** Để tìm kiếm và xóa thư email trong tổ chức của bạn, dễ nhất nếu bạn là quản trị viên toàn cầu. Nếu bạn không phải là quản trị viên toàn cầu, tài khoản của bạn sẽ được thêm vào nhóm vai trò quản lý eDiscovery hoặc vai trò quản lý tìm kiếm phù hợp. Để xóa thư, bạn sẽ cần tham gia nhóm vai trò quản lý tổ chức hoặc vai trò quản lý tìm kiếm và dọn sạch. Quyền cho các vai trò được chỉ định trong [Trung tâm tuân thủ & bảo mật](https://protection.office.com/).

1. [Tạo tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/content-search) để tìm thư cần xóa.
2. [Kết nối với bảo mật & tuân thủ trung tâm PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Nếu bạn đang sử dụng MFA, hãy xem [kết nối với Microsoft 365 security & tuân thủ trung tâm PowerShell bằng cách sử dụng xác thực nhiều yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
