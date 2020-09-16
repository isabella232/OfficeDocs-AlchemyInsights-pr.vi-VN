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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772320"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mã hóa thư email trong Outlook

Mã hóa thư Microsoft 365 được xây dựng trên Microsoft Azure Rights Management (Azure RMS), là một phần trong bảo vệ thông tin Azure. Nếu thuê bao của bạn bao gồm Azure rights management hoặc Azure Information Protection, **bạn không cần phải thực hiện bất kỳ hành động nào để bật hoặc kích hoạt** dịch vụ quản lý quyền theo cách thủ công.

Dựa trên phản hồi của khách hàng, chúng tôi sẽ không còn cho phép các quy tắc dòng thư Exchange để tự động mã hóa email có chứa một số loại thông tin nhạy cảm trong đối tượng thuê của bạn theo mặc định. Thay vào đó, chúng tôi đang cung cấp các hướng dẫn chi tiết về cách bạn có thể làm như vậy. Để biết thêm chi tiết về cách tạo quy tắc truyền dẫn để mã hóa thông tin nhạy cảm, hãy xem [bài viết này](https://aka.ms/OmeEtr).

- Nếu dùng Outlook trên web (trước đây là **OWA**): khi soạn thư email, chỉ cần bấm **bảo vệ** trong OWA. Quyền này sẽ áp dụng "không chuyển tiếp". Bấm vào **thay đổi quyền** và chọn **mã hóa** để chỉ mã hóa thư.

- Nếu dùng **Outlook Client**: để gửi thư được mã hóa từ Outlook 2013 hoặc 2016, hoặc Outlook 2016 for Mac, hãy chọn quyền **tùy chọn**  >  **Permissions**, sau đó chọn tùy chọn bảo vệ bạn cần.

- Để **tự động mã hóa tất cả email** được gửi đến một số người nhận nhất định hoặc các tổ chức đối tác bên ngoài, bạn cần tạo một quy tắc truyền dẫn dòng thư trong Trung tâm quản trị Exchange. Hướng dẫn chi tiết được cung cấp trong [bài viết hỗ trợ này](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

