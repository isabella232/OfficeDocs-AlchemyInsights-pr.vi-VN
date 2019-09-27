---
title: Nhãn độ nhạy không xuất hiện
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207247"
---
# <a name="sensitivity-labels-not-appearing"></a>Nhãn độ nhạy không xuất hiện

Nhãn nhạy cảm cho phép bạn phân loại và giúp bảo vệ nội dung nhạy cảm của mình. Chúng có thể được tạo ra trong Trung tâm tuân thủ Microsoft 365, Trung tâm bảo mật Microsoft 365 hoặc văn phòng 365 bảo mật & Trung tâm tuân thủ phân loại > độ nhạy nhãn. Để tìm hiểu thêm về tính năng này, hãy xem [tổng quan về các nhãn nhạy cảm](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Nếu bạn đã định cấu hình nhãn nhạy cảm nhưng chúng không xuất hiện trong các ứng dụng Office, hãy kiểm tra sau:

- Xác nhận rằng nhãn nhạy cảm đã được [xuất bản](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) cho người dùng và nhóm mà bạn muốn.

- Xác nhận rằng người dùng đang sử dụng một ứng dụng hỗ trợ nhãn nhạy cảm-xem [nhãn nhạy cảm trong tài liệu của bạn](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Nếu bạn đang [di chuyển các nhãn bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), hãy lưu ý các cân nhắc được liệt kê [ở đây](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Hỗ trợ ngăn mất dữ liệu (DLP): hiện tại, chỉ các nhãn lưu giữ có thể được sử dụng làm điều kiện trong chính sách DLP.  Hỗ trợ cho các nhãn nhạy cảm trong chính sách DLP không có sẵn nhưng chúng tôi đang làm việc trên đó.

- Khi mã hóa được bật trên nhãn nhạy cảm, bạn có thể chọn một trong hai cách:
    - Gán quyền ngay bây giờ
    - Cho phép người dùng chỉ định quyền


Để biết thêm thông tin về vấn đề có thể xảy ra, xem [các vấn đề với độ nhạy nhãn](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).