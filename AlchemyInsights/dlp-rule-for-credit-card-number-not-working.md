---
title: Quy tắc DLP cho Số Thẻ Tín dụng không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005112"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Sự cố DLP với số thẻ tín dụng

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Sự cố DLP với số thẻ tín dụng**

Bạn đang gặp sự cố với tính năng Ngăn  Mất Dữ liệu **(DLP)** không hoạt động đối với nội dung có chứa Số Thẻ Tín dụng khi sử dụng kiểu thông tin nhạy cảm DLP trong O365? Nếu vậy, hãy đảm bảo nội dung của bạn chứa thông tin cần thiết để kích hoạt chính sách DLP khi nó được đánh giá. Ví dụ,  đối với chính sách Thẻ Tín dụng được cấu hình với mức tin cậy 85%, thì những điều sau đây sẽ được đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 chữ số có thể được định dạng hoặc chưa định dạng (ddddddddddddd) và phải vượt qua kiểm tra Luquên.

- **[Mẫu hình:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mẫu hình rất phức tạp và mạnh mẽ giúp phát hiện thẻ từ tất cả các nhãn hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, thẻ quà tặng và thẻ mực.

- **[Kiểm tra:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Có, dấu kiểm Lubul

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Chính sách DLP tự tin rằng nó đã phát hiện ra loại thông tin nhạy cảm này nếu nằm trong khoảng cách 300 ký tự:

  - Hàm sẽ Func_credit_card nội dung khớp với mẫu hình.

  - Một trong những điều sau là đúng:

  - Tìm thấy từ Keyword_cc_verification từ khóa.

  - Tìm thấy từ Keyword_cc_name từ khóa

  - Hàm này Func_expiration_date thấy ngày ở định dạng ngày đúng.

  - Kiểm tra đi qua

    Ví dụ: mẫu sau đây sẽ kích hoạt cho Chính sách Số Thẻ Tín dụng DLP:

  - Visa: 4485 3647 3952 7352
  
  - Hết hạn: 02/02/2009

Để biết thêm thông tin  về những gì cần thiết để Số Thẻ Tín dụng được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: Kiểu Thông tin Nhạy cảm sẽ tìm kiếm Thẻ [Tín dụng#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Dùng một kiểu thông tin nhạy cảm khác nhau, hãy xem bài viết sau đây để biết thông tin về những gì được yêu cầu cho các kiểu khác: Kiểu Thông tin Nhạy cảm [sẽ tìm kiếm điều gì](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  