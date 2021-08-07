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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999694"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Cảnh báo email từ chính sách 'Chuyển phát thư lừa đảo do đối tượng thuê hoặc người dùng ghi đè'

Chính sách cảnh báo mặc định có tên "Giao hàng qua mạng do đối tượng thuê hoặc người dùng ghi đè" đã được triển khai cho các đối tượng thuê có giấy phép Microsoft Defender dành cho Office 365 P1 và P2. Nếu bạn nhận được cảnh báo này, dưới đây là các bước để điều tra:

1. Từ thông báo cảnh báo, hãy **bấm Xem Cảnh** báo để đến trang Cảnh báo **trong** Trung tâm Tuân & Chính sách Bảo mật.

2. Chọn cảnh báo để xem tùy chọn Xem **danh sách thư hoặc** Xem thư trong **Explorer**. Cả hai tùy chọn này sẽ đưa bạn đến chi tiết của thư, trong đó có ID Thông báo. Lưu ý rằng liên kết Trình khám phá Mối đe dọa sẽ tự động lọc các thư khớp với tiêu chí cảnh báo. Bạn có thể cần điều chỉnh bộ lọc ngày trong Trình khám phá Mối đe dọa.

Thư lừa đảo đã được chuyển phát do thay thế được cấu hình theo cách thủ công:

- Người dùng được phép đặt tên miền hoặc người dùng.

- Người gửi hoặc tên miền được phép thiết lập bởi người quản trị trong chính sách chống thư rác.

- Địa chỉ IP được cho phép trong chính sách bộ lọc kết nối.

- Quy tắc dòng thư (còn được gọi là quy tắc truyền tải) được cấu hình để cho phép thư nhập.

Nếu bạn cho rằng thư đã được đánh dấu sai [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) là thư lừa đảo qua điện thoại, hãy sử dụng phần bổ trợ Outlook Báo cáo để gửi mẫu thư đến Microsoft.
