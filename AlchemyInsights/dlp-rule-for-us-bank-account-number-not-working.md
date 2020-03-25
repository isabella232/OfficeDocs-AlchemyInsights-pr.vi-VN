---
title: Quy tắc DLP cho số tài khoản ngân hàng Hoa Kỳ không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932572"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

**Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ**

Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số tài khoản ngân hàng Hoa Kỳ** khi sử dụng loại thông tin nhạy cảm DLP trong O365? Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với chính sách **số tài khoản ngân hàng Hoa Kỳ** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 chữ số

- **[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 chữ số liên tiếp.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Biểu thức chính thông Regex_usa_bank_account_number tìm thấy nội dung phù hợp với mẫu

  - Tìm thấy từ khóa từ Keyword_usa_Bank_Account.

    Ví dụ, mẫu sau đây có kích hoạt cho chính sách **số tài khoản ngân hàng Hoa Kỳ** : kiểm tra tài khoản 78344011

Để biết thêm thông tin về những gì được yêu cầu cho một **số tài khoản ngân hàng Hoa Kỳ** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm kiếm số tài khoản ngân hàng Hoa Kỳ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  