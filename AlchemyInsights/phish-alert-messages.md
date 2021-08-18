---
title: 2491 Cảnh báo thư email từ chính sách 'Chuyển phát qua mạng do đối tượng thuê hoặc người dùng ghi đè'
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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316380"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Cảnh báo email từ chính sách 'Chuyển phát qua mạng do đối tượng thuê hoặc người dùng ghi đè'

Một chính sách  cảnh báo mặc định có tên Là lừa đảo qua mạng do đối tượng thuê hoặc người dùng ghi đè sẽ sẵn dùng trong các tổ chức có giấy phép Microsoft Defender dành Office 365 P1 và P2. Nếu bạn nhận được cảnh báo này, dưới đây là các bước để điều tra:

1. Từ thông báo cảnh báo, bấm **Xem Cảnh** báo để đi đến trang **Cảnh báo** trong cổng thông Bộ bảo vệ Microsoft 365 chính.

2. Chọn cảnh báo để xem tùy chọn Xem **danh sách thư hoặc** Xem thư trong **Explorer**. Cả hai tùy chọn này sẽ đưa bạn đến chi tiết của thư, trong đó có ID Thông báo. Lưu ý rằng liên kết Trình khám phá Mối đe dọa sẽ tự động lọc các thư khớp với tiêu chí cảnh báo. Bạn có thể cần điều chỉnh bộ lọc ngày trong Trình khám phá Mối đe dọa.

Thư lừa đảo đã được chuyển phát do thay thế được cấu hình theo cách thủ công:

- Người gửi hoặc tên miền được phép thiết lập bởi người dùng.
- Người gửi hoặc tên miền được phép được thiết lập bởi người quản trị trong chính sách chống thư rác.
- Địa chỉ IP được cho phép trong chính sách bộ lọc kết nối.
- Quy tắc dòng thư (còn được gọi là quy tắc truyền tải) được cấu hình để cho phép thư nhập.

Nếu bạn cho rằng thư đã bị đánh dấu sai là thư lừa đảo qua mạng, hãy sử dụng bản [gửi của Người quản](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) trị để báo cáo thư tới Microsoft.

Người dùng có thể [sử dụng](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) phần bổ trợ Thông báo Báo cáo hoặc phần bổ trợ Báo cáo Lừa đảo qua Outlook để gửi mẫu thư đến Microsoft.
