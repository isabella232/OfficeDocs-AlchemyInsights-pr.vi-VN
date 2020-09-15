---
title: 'AIP: chính sách không được điều hành như mong đợi'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663211"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: chính sách không được điều hành như mong đợi

Bảo vệ thông tin Azure: chính sách không được xử trị như mong đợi, hãy xem các hướng dẫn sau đây để được đề xuất cho các vấn đề chính sách khác nhau:

1. Nếu bạn đang gặp vấn đề với các dấu hiệu trực quan, vui lòng xem lại [khi áp dụng dấu hiệu trực quan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Nếu bạn đang gặp sự cố với việc ghi nhãn tự động, vui lòng xem lại [cách cấu hình các điều kiện cho việc phân loại thông tin và tự động cho Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các kiểu thông tin nhạy cảm tìm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)kiếm.
3. Nếu bạn đang gặp vấn đề với việc bảo vệ bản địa/Pfile, vui lòng xem lại [cấu hình API tệp](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kiểm tra xem bạn đang sử dụng các chính sách phạm vi không được cấu hình đúng cách: [cách đặt cấu hình chính sách bảo vệ thông tin Azure cho những người dùng cụ thể bằng cách sử dụng các chính sách giới hạn](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Nếu nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, hãy xác minh rằng Drmencryptthuộc tính không được xác định như được mô tả ở đây: [thiết đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Nếu bạn vẫn đang gặp phải vấn đề, vui lòng thu thập Nhật ký máy khách bảo vệ thông tin Azure và đính kèm các Nhật ký đã xuất ra vé này.

1. Mở tài liệu Office hoặc tạo email mới trong Outlook.
2. Bấm vào **bảo vệ/**  >  **Trợ giúp và phản hồi**nhạy cảm.
3. Bấm **xuất Nhật ký**.
4. Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ này.

Tài nguyên bổ sung:

- [Cách đặt cấu hình nhãn cho các dấu hiệu trực quan cho bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Xem lại tài liệu bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Sử dụng nhãn nhạy cảm trong ứng dụng Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

