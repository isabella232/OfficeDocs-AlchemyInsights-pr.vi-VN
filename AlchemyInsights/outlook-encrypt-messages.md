---
title: S/MIME trong Outlook trên web
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752882"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mã hóa thư email trong Outlook

Văn phòng 365 mã hóa thư được xây dựng trên Microsoft Azure quyền quản lý (Azure RMS), là một phần của Azure bảo vệ thông tin. Nếu đăng ký của bạn bao gồm quản lý quyền Azure hoặc bảo vệ thông tin Azure, **bạn không cần thực hiện bất kỳ hành động nào để bật hoặc kích hoạt** dịch vụ quản lý quyền theo cách thủ công.

Dựa trên phản hồi của khách hàng, chúng tôi sẽ không còn kích hoạt quy tắc luồng thư Exchange để tự động mã hóa email gửi đi có chứa một loại thông tin nhạy cảm nhất định trong đối tượng thuê của bạn theo mặc định. Thay vào đó, chúng tôi đang cung cấp hướng dẫn chi tiết về cách bạn có thể làm như vậy mình. Để biết thêm chi tiết về cách tạo quy tắc truyền tải để mã hóa thông tin nhạy cảm, xem [bài viết này](https://aka.ms/OmeEtr).

- Nếu sử dụng Outlook trên web (trước đây là **OWA**): khi soạn thư email, chỉ cần bấm **bảo vệ** trong OWA. Điều này sẽ áp dụng cho phép "không chuyển tiếp". Nhấp vào **thay đổi quyền** và chọn **mã hóa** chỉ để mã hóa thư.

- Nếu sử dụng **máy khách Outlook**: để gửi một tin nhắn được mã hóa từ Outlook 2013 hoặc 2016, hoặc Outlook 2016 cho Mac, chọn **tùy chọn** > **quyền**, sau đó chọn tùy chọn bảo vệ bạn cần.

- Để **tự động mã hóa tất cả email** được gửi đến người nhận nhất định hoặc các tổ chức đối tác bên ngoài, bạn cần tạo quy tắc truyền tải luồng thư trong Trung tâm quản trị Exchange. Hướng dẫn chi tiết được cung cấp trong [bài viết hỗ trợ này](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

