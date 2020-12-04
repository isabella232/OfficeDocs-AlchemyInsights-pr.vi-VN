---
title: Các khái niệm xác thực nâng cao áp dụng cho Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573782"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Các khái niệm xác thực nâng cao áp dụng cho Microsoft Edge

Sau đây là các khái niệm xác thực nâng cao được áp dụng cho Microsoft Edge:

**Xác thực chủ động**

Khi bạn bật chính sách được [kích hoạt Proactiveauth,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge sẽ cố gắng để xác thực chủ động cho người dùng được đăng nhập thông qua Microsoft Services. Tại các khoảng thời gian thường xuyên, nó sẽ sử dụng một dịch vụ trực tuyến để kiểm tra biểu thị được Cập Nhật có chứa xác thực chủ động quản lý cấu hình.

Lợi ích: xác thực chủ động cho phép xác thực cho các dịch vụ khóa, chẳng hạn như trang tab mới của Office. Ngoài ra, nếu Bing được dùng làm công cụ tìm kiếm, xác thực chủ động sẽ cải thiện hiệu suất của thanh địa chỉ và giúp tạo các kết quả tìm kiếm được cá nhân hóa với nhu cầu của doanh nghiệp của bạn.

**Windows Xin chào CredUI để xác thực NTLM**

Nếu đăng nhập đơn (SSO) không sẵn dùng khi một trang web cố gắng đăng nhập vào người dùng thông qua công trình NTLM hoặc thương lượng, tính năng này sẽ cho phép người dùng chia sẻ thông tin đăng nhập hệ điều hành với trang web và thỏa mãn thách thức xác thực bằng cách dùng Windows Hello cred UI. Dòng đăng nhập này sẽ chỉ xuất hiện trong Windows 10 và chỉ dành cho những người dùng không nhận được SSO trong một NTLM hoặc một thách thức thương lượng.

**Sử dụng mật khẩu đã lưu để đăng nhập tự động**

Người dùng lưu mật khẩu trong Microsoft Edge có thể bật tính năng đăng nhập tự động vào các trang web mà họ đã lưu chứng danh. Người dùng có thể bật hoặc tắt tính năng này trong edge://settings/passwords và bạn có thể cấu hình nó trong chính sách [trình quản lý mật khẩu](https://go.microsoft.com/fwlink/?linkid=2134622) .
