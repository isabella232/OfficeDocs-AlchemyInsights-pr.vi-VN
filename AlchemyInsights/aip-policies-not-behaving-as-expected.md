---
title: 'AIP: chính sách không phản bội như mong đợi'
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
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506580"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: chính sách không phản bội như mong đợi

Azure bảo vệ thông tin: chính sách không có như mong đợi, xem các hướng dẫn được khuyến nghị cho các vấn đề chính sách:

1. Nếu bạn đang gặp vấn đề với các dấu hiệu trực quan, vui lòng đánh giá [khi áp dụng](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)dấu hiệu hình ảnh.
2. Nếu bạn gặp sự cố với ghi nhãn tự động, vui lòng xem lại [cách cấu hình điều kiện để phân loại tự động và được đề xuất để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và [các loại thông tin nhạy cảm tìm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)kiếm.
3. Nếu bạn gặp vấn đề với Native/Pfile bảo vệ, hãy xem [tập tin cấu hình API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kiểm tra nếu bạn đang sử dụng chính sách scoped không được cấu hình đúng: [làm thế nào để cấu hình chính sách bảo vệ thông tin Azure cho người dùng cụ thể bằng cách sử dụng scoped chính sách](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Nếu ghi nhãn tự động không hoạt động cho Outlook khi đính kèm một tài liệu có nhãn, xác minh rằng DRMEncryptProperty không được xác định như mô tả ở đây: [cài đặt đăng ký IRM cho bảo mật](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Nếu bạn vẫn đang gặp sự cố, hãy thu thập Nhật ký khách hàng bảo vệ thông tin Azure và đính kèm Nhật ký xuất vé này.

1. Mở tài liệu Office hoặc tạo một email mới trong Outlook.
2. Nhấp vào **bảo vệ/**  >  **Trợ giúp độ nhạy và phản hồi**.
3. Nhấp vào **xuất Nhật ký**.
4. Lưu các bản ghi để lựa chọn vị trí của bạn, và đính kèm chúng vào yêu cầu dịch vụ này.

Tài nguyên bổ sung:

- [Làm thế nào để cấu hình nhãn cho dấu hiệu trực quan để bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Đánh giá tài liệu về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Sử dụng nhãn nhạy cảm trong ứng dụng Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

