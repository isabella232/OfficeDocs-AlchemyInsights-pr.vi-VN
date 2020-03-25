---
title: Quy tắc DLP cho số thẻ tín dụng không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932465"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP vấn đề với số thẻ tín dụng

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

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
  