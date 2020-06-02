---
title: Quy tắc DLP cho số tài khoản ngân hàng Hoa Kỳ không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507356"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ

**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ**

Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số tài khoản ngân hàng Hoa Kỳ** khi sử dụng loại thông tin nhạy cảm DLP trong O365? Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với chính sách **số tài khoản ngân hàng Hoa Kỳ** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 chữ số

- **[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 chữ số liên tiếp.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Biểu thức chính thông Regex_usa_bank_account_number tìm thấy nội dung phù hợp với mẫu

  - Tìm thấy từ khóa từ Keyword_usa_Bank_Account.

    Ví dụ, mẫu sau đây có kích hoạt cho chính sách **số tài khoản ngân hàng Hoa Kỳ** : kiểm tra tài khoản 78344011

Để biết thêm thông tin về những gì được yêu cầu cho một **số tài khoản ngân hàng Hoa Kỳ** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm kiếm số tài khoản ngân hàng Hoa Kỳ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  