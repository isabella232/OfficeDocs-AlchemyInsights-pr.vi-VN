---
title: Biểu tượng lịch không hiển thị trong máy khách nhóm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684720"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Biểu tượng lịch không hiển thị trong máy khách nhóm

Tab lịch trong nhóm yêu cầu quyền truy nhập vào hộp thư Exchange thông qua dịch vụ Web Exchange. Hộp thư Exchange có thể trực tuyến hoặc tại cơ sở. Đối với những người dùng trực tuyến không nhìn thấy tab lịch, hãy đảm bảo rằng chúng [được cấp phép cho hộp thư Exchange Online và hộp thư được bật](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Nếu người dùng có một hộp thư hợp lệ trong Exchange Online, nhưng vẫn không nhìn thấy tab lịch, bạn có thể gặp phải sự cố mạng. Sử dụng trình phân [tích kết nối từ xa của Microsoft](https://testconnectivity.microsoft.com/) và chạy các **kiểm tra kết nối dịch vụ web của Microsoft Exchange** cho người dùng bị ảnh hưởng.

Cuối cùng, hãy kiểm tra các [ứng dụng nhóm – chính sách thiết lập ứng dụng](https://admin.teams.microsoft.com/policies/app-setup) để đảm bảo rằng ứng dụng lịch chưa được loại bỏ khỏi chính sách được áp dụng cho người dùng (có thể là **mặc định toàn cầu (toàn**bộ tổ chức).

Nếu người dùng của bạn được sắp đặt tại cơ sở, bạn cần phải xác nhận cấu hình hỗn hợp của bạn được khỏe mạnh. Sử dụng trình [hướng dẫn cấu hình hỗn](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) hợp để khắc phục sự cố.

Lưu ý rằng các [nhóm yêu cầu Exchange 2016 CU3 hoặc cao hơn](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
