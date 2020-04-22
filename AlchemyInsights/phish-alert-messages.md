---
title: 2491 thông báo email từ ' phish gửi do thuê hoặc người dùng ghi đè ' chính sách
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758956"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Cảnh báo email từ ' phish Delivered do thuê hoặc người dùng ghi đè ' chính sách

Chính sách cảnh báo mặc định có tên "phish gửi do thuê hoặc người dùng ghi đè" đã được tung ra cho thuê với Office 365 ATP P1 và P2 giấy phép. Nếu bạn nhận được cảnh báo này, sau đây là các bước để điều tra:

1. Từ thông báo cảnh báo, nhấp vào **xem cảnh báo** để chuyển đến trang **cảnh báo** trong trung tâm tuân thủ & bảo mật.

2. Chọn cảnh báo để xem tùy chọn để **xem danh sách tin nhắn** hoặc **xem tin nhắn trong Explorer**. Cả hai tùy chọn này sẽ đưa bạn đến các chi tiết của thư, bao gồm thông báo ID. Lưu ý rằng liên kết Threat Explorer sẽ tự động lọc các thư phù hợp với tiêu chí cảnh báo. Bạn có thể cần phải điều chỉnh bộ lọc ngày trong Threat Explorer.

Thư lừa đảo đã được gửi do ghi đè cấu hình theo cách thủ công:

- Một người gửi hoặc miền được cho phép do người dùng đặt.

- Một người gửi hoặc tên miền được cho phép bởi quản trị viên trong chính sách chống thư rác.

- Một địa chỉ IP được phép trong chính sách lọc kết nối.

- Quy tắc lưu lượng thư (còn được gọi là quy tắc truyền tải) có cấu hình để cho phép thư.

Nếu bạn tin rằng thông báo không chính xác được đánh dấu là phish, sử dụng Outlook [báo cáo thông báo Add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) để gửi mẫu thư cho Microsoft.
