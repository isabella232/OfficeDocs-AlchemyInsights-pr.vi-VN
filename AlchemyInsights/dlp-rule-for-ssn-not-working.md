---
title: Quy tắc DLP SSN không làm việc
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320214"
---
Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **Số an sinh xã hội (SSN)** khi sử dụng một loại thông tin nhạy cảm trong Office 365? Nếu vậy, hãy chắc chắn rằng nội dung của bạn có chứa các thông tin cần thiết cho chính sách DLP là đang tìm kiếm. 
  
Ví dụ, cho một chính sách SSN, cấu hình với mức độ tin cậy là 85%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt:
  
- 9 **[định dạng:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** chữ số, có thể trong một mô hình định dạng hay định dạng 
    
- **[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn chức năng tìm kiếm SSNs trong bốn mẫu khác nhau: 
    
  - Func_ssn tìm thấy SSNs với pre-2011 mạnh định dạng được định dạng với dấu gạch ngang hoặc gian (ddd-dd-dddd OR ddd dd dddd)
    
  - Func_unformatted_ssn tìm thấy SSNs với pre-2011 mạnh định dạng được định dạng như chín chữ số liên tục (ddddddddd)
    
  - Func_randomized_formatted_ssn tìm thấy SSNs bài-2011 được định dạng với dấu gạch ngang hoặc gian (ddd-dd-dddd OR ddd dd dddd)
    
  - Func_randomized_unformatted_ssn tìm thấy SSNs bài-2011 được định dạng như chín chữ số liên tục (ddddddddd)
    
- **[Kiểm tra:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Không, đó là không có kiểm tra 
    
- **[Định nghĩa:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Một chính sách DLP là 85% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự: 
    
  - [Chức năng Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tìm thấy nội dung phù hợp với các mô hình. 
    
  - Tìm thấy một từ khóa từ [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Bao gồm các ví dụ của các từ khóa: *an sinh xã hội, an sinh xã hội #, Soc Sec, SSN* . Ví dụ, các mẫu sau sẽ kích hoạt chính sách DLP SSN: **SSN: 489-36-8350**
    
Để biết thêm chi tiết về những gì là cần thiết cho SSNs phát hiện cho nội dung của bạn, hãy xem phần sau đây trong bài viết này: [Những gì the nhạy cảm loại thông tin tìm kiếm SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  
