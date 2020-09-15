---
title: Phân loại tự động không được xử tại như mong muốn với máy khách AIP
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715223"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Phân loại tự động không được xử tại như mong muốn với máy khách AIP

Phân loại tự động không được xử trị như mong đợi, sử dụng các hướng dẫn được đề xuất sau đây:

1. Nếu bạn đang gặp sự cố với việc ghi nhãn tự động, hãy xem [làm thế nào để cấu hình các điều kiện cho việc phân loại tự động và đề xuất cho việc bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các kiểu thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kiểm tra xem bạn đang sử dụng các chính sách phạm vi không được cấu hình đúng cách: [cách đặt cấu hình chính sách bảo vệ thông tin Azure cho những người dùng cụ thể bằng cách sử dụng các chính sách giới hạn](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Nếu nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, hãy xác minh `DRMEncryptProperty` không được xác định như được mô tả ở đây: [thiết đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Nếu bạn đã sử dụng các [loại thông tin tích hợp sẵn](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) cho chính sách bảo vệ thông tin Azure của bạn, hãy xác nhận rằng nội dung của bạn khớp với định dạng dự kiến.
5. Xác minh rằng nhãn được cấu hình phù hợp cho **tự động** hoặc **đề**xuất. (Ghi nhãn**tự động** sẵn dùng cho tất cả các ứng dụng Microsoft 365, trong khi **đề** xuất sẵn dùng cho tất cả các ứng dụng Microsoft 365 ngoại trừ Outlook.)
6. Bạn không thể sử dụng tính năng phân loại tự động cho tài liệu và email trước đó đã được dán nhãn theo cách thủ công hoặc trước đó tự động được gắn nhãn với phân loại cao hơn.  Để biết thêm thông tin, hãy xem: [cách áp dụng nhãn tự động hoặc đề](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)xuất.
7. Nếu bạn vẫn gặp sự cố, vui lòng thu thập Nhật ký máy khách bảo vệ thông tin Azure và đính kèm các Nhật ký đã xuất vào phiếu hỗ trợ của bạn. Để xuất Nhật ký bảo vệ thông tin Azure:
    - Mở tài liệu Office hoặc tạo email mới trong Outlook.
    - Bấm vào **bảo vệ/**  >  **Trợ giúp và phản hồi**nhạy cảm.
    - Bấm **xuất Nhật ký**.
    - Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.

Để biết thêm thông tin, hãy xem:

- [Cách cấu hình các điều kiện cho phân loại tự động và được đề xuất cho bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Hướng dẫn cách làm cho các tình huống thông thường sử dụng bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Xem lại tài liệu bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Xem lại các gói đăng ký và tính năng bảo vệ thông tin Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Các yêu cầu về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hướng dẫn nhanh về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Tải xuống máy khách bảo vệ thông tin về Azure](https://www.microsoft.com/download/details.aspx?id=53018)
