---
title: Biểu tượng lịch không hiển thị trong Teams khách
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989613"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Biểu tượng lịch không hiển thị trong Teams khách

Tab Lịch trong Thư Teams yêu cầu quyền truy nhập vào một hộp Exchange thông qua Exchange Vụ Web. Hộp Exchange của bạn có thể là Trực tuyến hoặc Tại chỗ. Đối với người dùng Trực tuyến không nhìn thấy Tab Lịch, hãy đảm bảo rằng họ được cấp phép cho hộp [thư Exchange Online và hộp thư được bật](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Nếu người dùng có một hộp thư hợp lệ trong Exchange Online nhưng vẫn không thể nhìn thấy tab Lịch, bạn có thể gặp phải một vấn đề về mạng. Sử dụng [Trình phân tích Kết nối Từ xa của](https://testconnectivity.microsoft.com/) Microsoft và chạy Kiểm tra Kết nối Dịch vụ Web của Microsoft Exchange **cho** người dùng bị ảnh hưởng.

Cuối cùng hãy kiểm [tra Teams Apps –](https://admin.teams.microsoft.com/policies/app-setup) Chính sách thiết lập ứng dụng để đảm bảo ứng dụng Lịch không bị loại bỏ khỏi chính sách được áp dụng cho người dùng (rất có thể là Toàn cầu (Mặc định trong toàn tổ **chức).**

Nếu người dùng của bạn được đặt tại chỗ, bạn cần xác nhận cấu hình Kết hợp của mình hoạt động tốt. Sử dụng Trình hướng [dẫn Cấu hình Kết hợp](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) để khắc phục sự cố.

Lưu ý [rằng Teams cần Exchange CU3 2016 trở lên.](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)
