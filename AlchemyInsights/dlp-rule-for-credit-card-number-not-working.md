---
title: Quy tắc DLP cho số thẻ tín dụng không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704223"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP vấn đề với số thẻ tín dụng

**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**DLP vấn đề với số thẻ tín dụng**

Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa **số thẻ tín dụng** khi sử dụng loại thông tin nhạy cảm DLP trong O365? Nếu có, đảm bảo rằng nội dung của bạn chứa thông tin cần thiết để kích hoạt chính sách DLP khi nó được đánh giá. Ví dụ: đối với **chính sách thẻ tín dụng** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chữ số mà có thể được định dạng hoặc định dạng (dddddddddddddddd) và phải vượt qua các thử nghiệm Luhn.

- **[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Rất phức tạp và mạnh mẽ mô hình phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, thẻ quà tặng, và thẻ Diner.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Có, kiểm tra Luhn

- **[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Chính sách DLP là 85% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Chức năng Func_credit_card tìm thấy nội dung phù hợp với mẫu.

  - Một trong những việc sau đây là đúng:

  - Một từ khóa từ Keyword_cc_verification được tìm thấy.

  - Một từ khóa từ Keyword_cc_name được tìm thấy

  - Chức năng Func_expiration_date tìm thấy một ngày ở định dạng ngày đúng.

  - Checksum đi qua

    Ví dụ, mẫu sau đây có kích hoạt cho chính sách số thẻ tín dụng DLP:

  - Thị thực: 4485 3647 3952 7352
  
  - Hết hạn: 2/2009

Để biết thêm thông tin về những gì được yêu cầu cho một **số thẻ tín dụng** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những gì các loại thông tin nhạy cảm tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  