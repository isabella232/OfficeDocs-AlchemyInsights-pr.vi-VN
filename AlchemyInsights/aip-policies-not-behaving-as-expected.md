---
title: 'AIP: Các chính sách không có tác dụng như mong đợi'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934315"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Các chính sách không có tác dụng như mong đợi

Azure Information Protection: Các chính sách không có tác dụng như mong đợi, hãy xem các nội dung sau để biết các hướng dẫn được đề xuất cho các sự cố chính sách khác nhau:

1. Nếu bạn đang gặp vấn đề với đánh dấu trực quan, vui lòng xem [lại Khi nào áp dụng các đánh dấu trực quan.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Nếu bạn đang gặp sự cố với dán nhãn tự động, vui lòng xem lại Cách đặt cấu hình các điều kiện để phân loại tự động và được đề xuất cho [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) và loại thông tin nhạy cảm sẽ tìm kiếm những [gì.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Nếu bạn đang gặp sự cố với bảo vệ Native/Pfile, vui lòng xem lại [cấu hình API Tệp](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kiểm tra xem bạn có đang dùng các chính sách thuộc phạm vi không được cấu hình đúng hay không: Cách cấu hình chính sách Azure Information Protection cho người dùng cụ thể bằng cách sử dụng các [chính sách theo phạm vi.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Nếu tính năng dán nhãn tự động không hoạt động đối với Outlook khi đính kèm một tài liệu có nhãn, hãy xác nhận rằng DRMEncryptProperty không được xác định như mô tả ở đây: Thiết đặt sổ đăng ký [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)cho bảo mật.

Nếu bạn vẫn gặp sự cố, vui lòng thu thập nhật ký máy khách Azure Information Protection và đính kèm các nhật ký đã xuất vào vé này.

1. Mở tài Office hoặc tạo email mới trong Outlook.
2. Bấm Bảo **vệ/Trợ giúp Nhạy**  >  **Cảm và phản hồi.**
3. Bấm **Xuất Nhật ký.**
4. Lưu nhật ký vào lựa chọn của bạn về vị trí và đính kèm nhật ký vào yêu cầu dịch vụ này.

Các tài nguyên bổ sung:

- [Cách đặt cấu hình nhãn cho dấu hiệu trực quan cho Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Xem lại hướng dẫn sử dụng Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Sử dụng nhãn nhạy cảm trong các Microsoft 365 dụng](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

