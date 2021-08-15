---
title: Phân loại tự động không hoạt động như dự kiến với máy khách AIP
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
- "9002266"
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979731"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Phân loại tự động không hoạt động như dự kiến với máy khách AIP

Phân loại tự động không có hành vi như mong đợi, hãy sử dụng các hướng dẫn được đề xuất sau đây:

1. Nếu bạn đang gặp sự cố với dán nhãn tự động, hãy xem mục Cách đặt cấu hình các điều kiện để phân loại tự động và được đề xuất cho [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và loại thông tin nhạy cảm sẽ tìm kiếm những [gì.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Kiểm tra xem bạn có đang dùng các chính sách thuộc phạm vi không được cấu hình đúng hay không: Cách cấu hình chính sách Azure Information Protection cho người dùng cụ thể bằng cách sử dụng các [chính sách theo phạm vi.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Nếu tính năng dán nhãn tự động không hoạt động Outlook khi đính kèm tài liệu có nhãn, hãy xác nhận rằng điều đó không được xác định như mô tả ở đây: Thiết đặt sổ đăng ký IRM cho bảo `DRMEncryptProperty` [mật.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Nếu bạn đã sử dụng các [kiểu thông tin tích hợp sẵn cho](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) chính sách Azure Information Protection của mình, hãy xác minh rằng nội dung của bạn khớp với định dạng dự kiến.
5. Xác nhận rằng nhãn đã được đặt cấu hình phù hợp cho Tự **động hoặc** Đề **xuất.** (**Tự động** đánh nhãn sẵn dùng cho  tất cả các Microsoft 365, trong khi được đề xuất sẵn dùng cho tất cả các ứng Microsoft 365 ngoại trừ Outlook.)
6. Bạn không thể sử dụng phân loại tự động cho các tài liệu và email trước đây được đánh nhãn theo cách thủ công hoặc trước đây có nhãn tự động kèm theo phân loại cao hơn.  Để biết thêm thông tin, hãy xem: [Cách áp dụng nhãn tự](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)động hoặc được đề xuất .
7. Nếu bạn vẫn gặp phải sự cố, vui lòng thu thập nhật ký máy khách Azure Information Protection và đính kèm nhật ký đã xuất vào vé hỗ trợ của bạn. Để xuất nhật ký Azure Information Protection:
    - Mở tài Office hoặc tạo email mới trong Outlook.
    - Bấm Bảo **vệ/Trợ giúp Nhạy**  >  **Cảm và phản hồi.**
    - Bấm **Xuất Nhật ký.**
    - Lưu nhật ký vào lựa chọn của bạn về vị trí và đính kèm nhật ký vào yêu cầu dịch vụ của bạn.

Để biết thêm thông tin, hãy xem:

- [Cách đặt cấu hình các điều kiện cho phân loại tự động và được đề xuất cho Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Hướng dẫn cách thực hiện cho các kịch bản phổ biến sử dụng Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Xem lại hướng dẫn sử dụng Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Xem lại các đăng ký và tính năng Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Yêu cầu đối với Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hướng dẫn nhanh về Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Tải xuống máy khách Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
