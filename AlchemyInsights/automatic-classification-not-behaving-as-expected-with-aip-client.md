---
title: Tự động phân loại không cư xử như mong đợi với khách hàng AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493441"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Tự động phân loại không cư xử như mong đợi với khách hàng AIP

Phân loại tự động không có như mong đợi, sử dụng các hướng dẫn được khuyến nghị sau:

1. Nếu bạn gặp sự cố với ghi nhãn tự động, hãy xem [cách cấu hình điều kiện để phân loại tự động và được đề xuất để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Kiểm tra nếu bạn đang sử dụng chính sách scoped không được cấu hình đúng: [làm thế nào để cấu hình chính sách bảo vệ thông tin Azure cho người dùng cụ thể bằng cách sử dụng scoped chính sách](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Nếu ghi nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, xác minh rằng `DRMEncryptProperty` không được xác định như mô tả ở đây: [cài đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Nếu bạn đã sử dụng các [loại thông tin tích hợp](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) cho chính sách bảo vệ thông tin Azure của bạn, hãy xác minh rằng nội dung của bạn phù hợp với định dạng mong muốn.
5. Xác minh rằng nhãn được cấu hình phù hợp cho **tự động** hoặc **khuyến nghị**. (Ghi nhãn**tự động** có sẵn cho tất cả các ứng dụng Office, trong khi **đề xuất** có sẵn cho tất cả các ứng dụng Office ngoại trừ Outlook.)
6. Bạn không thể sử dụng phân loại tự động cho các tài liệu và email trước đây được gắn nhãn theo cách thủ công hoặc trước đây tự động gắn nhãn với phân loại cao hơn.  Để biết thêm thông tin, xem: [làm thế nào tự động hoặc khuyến cáo nhãn được áp dụng](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Nếu bạn vẫn gặp sự cố, hãy thu thập Nhật ký khách hàng bảo vệ thông tin Azure và đính kèm Nhật ký xuất vé hỗ trợ của bạn. Xuất Nhật ký Azure thông tin bảo vệ:
    - Mở tài liệu Office hoặc tạo một email mới trong Outlook.
    - Nhấp vào **bảo vệ/**  >  **Trợ giúp độ nhạy và phản hồi**.
    - Nhấp vào **xuất Nhật ký**.
    - Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.

Để biết thêm thông tin, xem:

- [Cách cấu hình điều kiện để phân loại tự động và được đề xuất để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Hướng dẫn cách để các trường hợp phổ biến sử dụng bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Đánh giá tài liệu về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Review Azure bảo vệ thông tin đăng ký và tính năng](https://azure.microsoft.com/pricing/details/information-protection)
- [Yêu cầu đối với bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hướng dẫn bắt đầu nhanh để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Tải về Azure bảo vệ thông tin khách hàng](https://www.microsoft.com/download/details.aspx?id=53018)
