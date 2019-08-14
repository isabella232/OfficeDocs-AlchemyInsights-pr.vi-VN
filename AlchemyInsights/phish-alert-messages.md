---
title: 2491 email cảnh báo tin nhắn từ chính sách 'Phish giao hàng do người thuê nhà hoặc người dùng ghi đè
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391628"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Các thư email cảnh báo từ chính sách 'Phish giao hàng do người thuê nhà hoặc người dùng ghi đè

Một chính sách mặc định cảnh báo tên "Phish Delivered do người thuê nhà hoặc người dùng ghi đè" đã được cán cho người thuê nhà với giấy phép Office 365 ATP P1 và P2. Nếu bạn nhận được thông báo này, dưới đây là các bước điều tra:

1. Từ cảnh báo, hãy nhấp vào **Xem thông báo** để đi đến trang **cảnh báo** an ninh & Trung tâm phù hợp.

2. Chọn cảnh báo để xem các tùy chọn để **xem thông báo danh sách** hoặc **xem tin nhắn trong Explorer**. Cả hai các tùy chọn này sẽ đưa bạn đến các chi tiết của thư, bao gồm ID tin nhắn Lưu ý rằng các liên kết mối đe dọa Explorer sẽ tự động lọc thư phù hợp với các tiêu chí cảnh báo. Bạn có thể cần phải điều chỉnh các bộ lọc ngày trong Explorer mối đe dọa.

Thư lừa đảo đã được chuyển giao bởi vì một ghi đè cấu hình thủ công:

- Cho phép người gửi hay tên miền thiết lập bởi người dùng.

- Cho phép người gửi hay tên miền thiết lập bởi các quản trị viên trong một chính sách chống thư rác.

- Một địa chỉ IP được cho phép trong một chính sách lọc kết nối.

- Một luồng quy tắc thư (cũng được biết đến như là một quy tắc truyền tải) được cấu hình để cho phép các tin nhắn trong.

Nếu bạn tin rằng thư được đánh dấu không chính xác như phish, sử dụng các Outlook [tin nhắn báo cáo add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) để gửi thông báo mẫu cho Microsoft.
