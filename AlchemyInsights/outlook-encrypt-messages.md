---
title: S/MIME trong Outlook trên web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010746"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mã hóa thư email trong Outlook

Microsoft 365 Mã hóa Thư được xây dựng trên Microsoft Azure Rights Management (Azure RMS), vốn là một phần của Azure Information Protection. Nếu đăng ký của bạn bao gồm Azure Rights Management hoặc Azure Information **Protection,** bạn không cần thực hiện bất kỳ hành động nào để bật hoặc kích hoạt Dịch vụ Quản trị Quyền theo cách thủ công.

Dựa trên phản hồi của khách hàng, chúng tôi sẽ không còn cho phép quy tắc dòng thư Exchange tự động mã hóa email gửi đi có chứa một số loại thông tin nhạy cảm nhất định trong đối tượng thuê của bạn theo mặc định. Thay vào đó, chúng tôi sẽ cung cấp các hướng dẫn chi tiết về cách bạn có thể tự thực hiện. Để biết thêm chi tiết về cách tạo quy tắc truyền dẫn để mã hóa thông tin nhạy cảm, hãy xem [bài viết này.](https://aka.ms/OmeEtr)

- Nếu sử Outlook trên Web (trước đây là **OWA**): Khi soạn thư email, chỉ cần bấm **vào Bảo vệ** trong OWA. Điều này sẽ áp dụng quyền "Không chuyển tiếp". Bấm **Thay đổi quyền** và chọn Mã **hóa** để chỉ mã hóa thư.

- Nếu sử **dụng Outlook client**: Để gửi thư được mã hóa từ Outlook 2013 hoặc 2016 hoặc Outlook 2016 for Mac, hãy chọn Quyền Tùy chọn , sau đó chọn tùy chọn bảo vệ bạn   >  cần.

- Để **tự động mã** hóa tất cả email được gửi đến một số người nhận nhất định hoặc tổ chức đối tác bên ngoài, bạn cần tạo quy tắc truyền tải dòng thư trong Trung tâm Quản Exchange Của bạn. Hướng dẫn chi tiết được cung cấp [trong bài viết hỗ trợ này.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

