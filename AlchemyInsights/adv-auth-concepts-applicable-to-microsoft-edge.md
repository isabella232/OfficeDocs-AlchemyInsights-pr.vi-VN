---
title: Các khái niệm xác thực nâng cao có thể áp Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934387"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Các khái niệm xác thực nâng cao có thể áp Microsoft Edge

Sau đây là các khái niệm xác thực nâng cao có thể áp dụng cho các Microsoft Edge:

**Xác thực Chủ động**

Khi bạn bật chính [sách Chủ](https://go.microsoft.com/fwlink/?linkid=2134621) động Xác thực Được xác thực, Microsoft Edge sẽ cố gắng chủ động xác thực người dùng đã đăng nhập thông qua dịch vụ Microsoft. Theo định kỳ, nó sẽ sử dụng một dịch vụ trực tuyến để kiểm tra tệp kê khai được cập nhật có chứa cấu hình quản lý Xác thực Chủ động.

Lợi ích: Xác thực Chủ động cho phép xác thực đối với các dịch vụ chính, chẳng hạn Office Trang Tab Mới. Ngoài ra, nếu Bing dùng làm công cụ tìm kiếm, tính năng Xác thực Chủ động cũng sẽ cải thiện hiệu suất của thanh địa chỉ và giúp tạo kết quả tìm kiếm cá nhân hóa cho nhu cầu của doanh nghiệp bạn.

**Windows Hello CredUI cho Xác thực NTLM**

Nếu đăng nhập đơn (SSO) không sẵn dùng khi một website cố gắng đăng nhập vào người dùng thông qua cơ chế NTLM hoặc Đàm phán, tính năng này sẽ cho phép người dùng chia sẻ thông tin xác thực HĐH với website và thỏa mãn thử thách xác thực bằng cách sử dụng giao diện người dùng Windows Hello Cred. Dòng đăng nhập này sẽ chỉ xuất hiện trong Windows 10 và chỉ dành cho người dùng không nhận được SSO khi gặp NTLM hoặc thử thách Đã đàm phán.

**Sử dụng mật khẩu đã lưu để đăng nhập tự động**

Người dùng lưu mật khẩu trong Microsoft Edge thể bật tính năng đăng nhập tự động vào các website mà họ đã lưu thông tin xác thực. Người dùng có thể bật hoặc tắt tính năng này trong edge://settings/passwords và bạn có thể cấu hình tính năng này trong chính sách của người [quản lý mật](https://go.microsoft.com/fwlink/?linkid=2134622) khẩu.
