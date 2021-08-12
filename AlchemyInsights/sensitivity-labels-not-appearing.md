---
title: Nhãn nhạy cảm không xuất hiện
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061454"
---
# <a name="sensitivity-labels-not-appearing"></a>Nhãn nhạy cảm không xuất hiện

Nhãn nhạy cảm cho phép bạn phân loại và giúp bảo vệ nội dung nhạy cảm của bạn. Chúng có thể được tạo trong Trung tâm Bảo mật Trung tâm tuân thủ Microsoft 365, Microsoft 365 hoặc Trung tâm Bảo mật Microsoft 365 & Tuân thủ thuộc Phân loại > Nhãn nhạy cảm. Để tìm hiểu thêm về tính năng này, hãy [xem Tổng quan về nhãn nhạy cảm.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Nếu bạn cấu hình nhãn nhạy cảm nhưng chúng không xuất hiện trong ứng dụng Microsoft 365, hãy kiểm tra các mục sau:

- Xác nhận rằng nhãn nhạy cảm đã được [phát](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) hành cho người dùng và nhóm mà bạn muốn.

- Xác nhận rằng người dùng đang dùng ứng dụng hỗ trợ nhãn nhạy cảm - xem nhãn [nhạy cảm trong tài liệu của bạn](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Nếu bạn đang di [chuyển các nhãn Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), hãy lưu ý những điều cần cân nhắc được liệt kê ở [đây.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Hỗ trợ Ngăn mất dữ liệu (DLP) Hiện tại, chỉ có thể dùng nhãn duy trì làm điều kiện trong chính sách DLP.  Hỗ trợ cho nhãn nhạy cảm trong chính sách DLP chưa sẵn có nhưng chúng tôi đang nghiên cứu cách làm.

- Khi mã hóa được bật trên nhãn nhạy cảm, bạn có thể chọn:
    - Gán quyền ngay bây giờ
    - Cho phép người dùng gán quyền


Để biết thêm thông tin về các vấn đề có thể xảy [ra, hãy xem Các vấn đề đã biết với nhãn nhạy cảm](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).