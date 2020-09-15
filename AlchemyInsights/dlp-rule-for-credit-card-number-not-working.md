---
title: Quy tắc số thẻ tín dụng không hoạt động
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679463"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Các vấn đề về các số thẻ tín dụng

**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Các vấn đề về các số thẻ tín dụng**

Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung chứa một **số thẻ tín dụng** khi sử dụng kiểu thông tin nhạy cảm trong O365? Nếu vậy, hãy đảm bảo rằng nội dung của bạn có chứa thông tin cần thiết để kích hoạt chính sách được phát hiện khi nó được đánh giá. Ví dụ: đối với một **chính sách thẻ tín dụng** được cấu hình với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 chữ số có thể được định dạng hoặc không được định dạng (dddddddddddddddddddddddd) và phải vượt qua kiểm tra Luhn.

- **[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mẫu rất phức tạp và mạnh mẽ mà phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards và Diner cards.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Có, checksum Luhn

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Chính sách có thể là 85% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Hàm Func_credit_card tìm thấy nội dung khớp với mẫu.

  - Một trong những điều sau là đúng:

  - Tìm thấy một từ khóa từ Keyword_cc_verification.

  - Một từ khóa từ Keyword_cc_name được tìm thấy

  - Hàm Func_expiration_date tìm thấy một ngày trong định dạng ngày bên phải.

  - Bộ kiểm tra vượt quá

    Ví dụ, mẫu sau sẽ kích hoạt cho chính sách số thẻ tín dụng đã định vị:

  - Visa: 4485 3647 3952 7352
  
  - Hết hạn: 2/2009

Để biết thêm thông tin về yêu cầu **số thẻ tín dụng** được phát hiện đối với nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm cần tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  