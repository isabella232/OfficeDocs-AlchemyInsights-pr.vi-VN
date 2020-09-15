---
title: Quy tắc định đối với SSN không hoạt động
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679391"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Các vấn đề về số an sinh xã hội

**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Các vấn đề về việc có SSNs**

Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung chứa **số an sinh xã hội (SSN)** khi sử dụng kiểu thông tin nhạy cảm trong Microsoft 365? Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm. 
  
Ví dụ: đối với một chính sách SSN được cấu hình với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 chữ số, trong đó có thể có trong một mẫu có định dạng hoặc chưa định dạng

- **[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn hàm Look cho SSNs trong bốn mẫu khác nhau:

  - Func_ssn tìm thấy các SSNs với định dạng mạnh 2011 được định dạng bằng dấu gạch ngang hoặc dấu cách (DDD-dd-dddd hoặc DDD dd dddd)

  - Func_unformatted_ssn tìm thấy các SSNs với định dạng mạnh 2011 được bỏ định dạng dưới dạng chín chữ số liên tiếp (ddddddddd)

  - Func_randomized_formatted_ssn tìm thấy Post-2011 SSNs được định dạng bằng dấu gạch ngang hoặc dấu cách (DDD-dd-dddd hoặc DDD dd dddd)

  - Func_randomized_unformatted_ssn tìm thấy Post-2011 SSNs không được định dạng dưới dạng chín chữ số liên tiếp (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Chính sách có thể là 85% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - [Hàm Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) tìm thấy nội dung khớp với mẫu.

  - Tìm thấy một từ khóa từ [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Ví dụ về từ khóa bao gồm:  *an sinh xã hội, số an sinh xã hội #, SoC SEC, SSN*  . Ví dụ, mẫu sau sẽ được kích hoạt cho chính sách định vị: **SSN: 489-36-8350**
  
Để biết thêm thông tin về những điều cần thiết cho SSNs được phát hiện đối với nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm cần tìm kiếm SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  