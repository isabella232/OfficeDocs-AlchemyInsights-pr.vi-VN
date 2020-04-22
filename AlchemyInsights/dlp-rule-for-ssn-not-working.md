---
title: Quy tắc DLP cho SSN không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704107"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Các vấn đề DLP với số an ninh xã hội

**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

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
  