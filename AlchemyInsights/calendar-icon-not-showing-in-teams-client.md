---
title: Biểu tượng lịch không hiển thị trong khách hàng teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932379"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Biểu tượng lịch không hiển thị trong khách hàng teams

Tab lịch trong teams yêu cầu quyền truy cập vào hộp thư Exchange qua dịch vụ Web Exchange. Hộp thư Exchange có thể trực tuyến hoặc tại chỗ. Đối với người dùng trực tuyến không thấy tab lịch, đảm bảo rằng chúng [được cấp phép cho hộp thư Exchange Online và hộp thư được kích hoạt](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Nếu người dùng có một hộp thư hợp lệ trong Exchange Online, nhưng vẫn không thể xem tab lịch, bạn có thể gặp sự cố mạng. Sử dụng [phân tích kết nối từ xa của Microsoft](https://testconnectivity.microsoft.com/) và chạy **kiểm tra kết nối dịch vụ web của Microsoft Exchange** cho người dùng bị ảnh hưởng.

Cuối cùng kiểm tra các [ứng dụng teams-chính sách thiết lập ứng dụng](https://admin.teams.microsoft.com/policies/app-setup) để đảm bảo ứng dụng lịch không bị xóa khỏi chính sách được áp dụng cho người dùng (nhiều khả năng là **toàn cầu (mặc định**trong toàn bộ).

Nếu người dùng của bạn homed tại chỗ, bạn cần xác nhận cấu hình kết hợp của bạn là ổn định. Sử dụng [thuật sĩ cấu hình kết](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) hợp để khắc phục sự cố.

Lưu ý rằng các [nhóm yêu cầu Exchange 2016 CU3 trở](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)lên.
