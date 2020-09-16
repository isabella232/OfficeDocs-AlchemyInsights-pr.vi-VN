---
title: 2491 thông báo email từ ' phish Delivered do chính sách đối tượng thuê hoặc ghi đè người dùng
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728633"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Thông báo tin nhắn email từ ' phish Delivered do chính sách đối tượng thuê hoặc ghi đè người dùng

Một chính sách cảnh báo mặc định có tên là "phish được chuyển phát do đối tượng thuê hoặc người dùng ghi đè" đã được triển khai cho các đối tượng thuê với Office 365 ATP P1 và P2 giấy phép. Nếu bạn nhận được cảnh báo này, sau đây là các bước để điều tra:

1. Từ thông báo cảnh báo, hãy bấm **xem cảnh báo** để đi đến trang **cảnh báo** trong trung tâm tuân thủ & bảo mật.

2. Chọn cảnh báo để xem tùy chọn để **xem danh sách thư** hoặc **xem thư trong Explorer**. Cả hai tùy chọn này sẽ đưa bạn đến chi tiết của thư, trong đó bao gồm ID thư. Lưu ý rằng nối kết mối đe dọa Explorer sẽ tự động lọc các thư khớp với tiêu chí cảnh báo. Bạn có thể cần điều chỉnh bộ lọc ngày trong Threat Explorer.

Thư lừa đảo được chuyển phát do ghi đè được cấu hình thủ công:

- Người dùng hoặc tên miền được cho phép.

- Người gửi hoặc tên miền được cho phép do người quản trị thiết lập trong chính sách chống thư rác.

- Một địa chỉ IP được cho phép trong chính sách bộ lọc kết nối.

- Quy tắc dòng thư (còn được gọi là quy tắc truyền dẫn) được cấu hình để cho phép các thư trong đó.

Nếu bạn tin rằng thư không được đánh dấu là phish, hãy dùng [bổ trợ tin nhắn báo cáo](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook để gửi mẫu thư vào Microsoft.
