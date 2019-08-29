---
title: S/MIME trong Outlook trên web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666862"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mật mã hóa các tin nhắn email trong Outlook

Office 365 thư mã hóa được xây dựng trên Microsoft Azure quản lý quyền (Azure RMS), là một phần của bảo vệ thông tin Azure. Nếu thuê bao của bạn bao gồm Azure quyền quản lý hoặc bảo vệ thông tin Azure, **bạn không cần phải thực hiện bất kỳ hành động để tự kích hoạt hoặc kích hoạt** dịch vụ quản lý quyền.

Dựa trên thông tin phản hồi của khách hàng, chúng tôi sẽ không còn tạo điều kiện cho quy tắc lưu lượng trao đổi thư để tự động mã hóa email gửi đi có chứa một số loại thông tin nhạy cảm ở người thuê nhà của bạn theo mặc định. Thay vào đó, chúng tôi đang cung cấp hướng dẫn chi tiết về làm thế nào bạn có thể làm như vậy chính mình. Để biết thêm chi tiết về làm thế nào để tạo một quy tắc truyền tải để mã hóa thông tin nhạy cảm, xem [bài viết này](https://aka.ms/OmeEtr).

- Nếu sử dụng Outlook trên Web (formerly **OWA**): khi soạn một tin nhắn email, chỉ cần nhấp vào **bảo vệ** trong OWA. Điều này sẽ áp dụng quyền "Làm không chuyển tiếp". Nhấp vào **thay đổi quyền** và chọn **mã hoá** chỉ mật mã hóa thư.

- Nếu sử dụng **Outlook client**: để gửi một tin nhắn được mã hóa từ Outlook 2013 hay 2016 hoặc Outlook 2016 cho Mac, chọn **tùy chọn** > **quyền**, sau đó chọn tùy chọn bảo vệ mà bạn cần.

- Để **tự động mã hóa tất cả các email** được gửi đến người nhận hoặc tổ chức đối tác bên ngoài nhất định, bạn cần phải tạo một quy tắc truyền tải lưu lượng thư trong Trung tâm quản trị Exchange. Hướng dẫn chi tiết được cung cấp trong [bài viết hỗ trợ này](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

