---
title: Quy tắc DLP cho SSN không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932561"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Các vấn đề DLP với số an ninh xã hội

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

**Vấn đề DLP với SSNs**

Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa **số an ninh xã hội (SSN)** khi sử dụng một loại thông tin nhạy cảm trong Office 365? Nếu vậy, hãy đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm. 
  
Ví dụ: đối với một chính sách SSN được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 chữ số, trong đó có thể là một mẫu định dạng

- **[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn chức năng tìm kiếm SSNs trong bốn mô hình khác nhau:

  - Func_ssn thấy SSNs với Pre-2011 định dạng mạnh được định dạng với dấu gạch ngang hoặc không gian (DDD-dd-dddd hoặc DDD dd dddd)

  - Func_unformatted_ssn tìm thấy SSNs với Pre-2011 định dạng mạnh mẽ mà không thể bỏ là chín chữ số liên tiếp (ddddddddd)

  - Func_randomized_formatted_ssn tìm thấy bài viết-2011 SSNs được định dạng với dấu gạch ngang hoặc không gian (DDD-dd-dddd hoặc DDD dd dddd)

  - Func_randomized_unformatted_ssn tìm thấy bài đăng-2011 SSNs được định dạng là chín chữ số liên tiếp (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Chính sách DLP là 85% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - [Chức năng Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tìm thấy nội dung phù hợp với mẫu.

  - Từ khóa từ [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) được tìm thấy. Ví dụ về các từ khóa bao gồm: *an ninh xã hội, an ninh xã hội #, SoC SEC, SSN* . Ví dụ, mẫu sau đây có kích hoạt cho chính sách DLP SSN: **SSN: 489-36-8350**
  
Để biết thêm thông tin về những gì được yêu cầu cho SSNs được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm kiếm SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  