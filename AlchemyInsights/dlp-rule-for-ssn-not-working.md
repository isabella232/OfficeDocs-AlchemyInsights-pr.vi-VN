---
title: Quy tắc DLP cho SSN không hoạt động
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005004"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Sự cố DLP với Số An sinh Xã hội

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Sự cố DLP với các SSN**

Bạn đang gặp sự cố với tính năng Ngăn Mất Dữ liệu **(DLP)** không hoạt động đối với nội dung có chứa Số An sinh Xã hội **(SSN)** khi sử dụng kiểu thông tin nhạy cảm trong Microsoft 365? Nếu vậy, hãy đảm bảo rằng nội dung của bạn chứa các thông tin cần thiết cho nội dung chính sách DLP đang tìm kiếm. 
  
Ví dụ, đối với một chính sách SSN được cấu hình với mức tin cậy 85%, các điều sau đây được đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 chữ số, có thể theo mẫu hình có định dạng hoặc không định dạng

- **[Mẫu hình:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn hàm tìm kiếm SSN theo bốn mẫu hình khác nhau:

  - Func_ssn sẽ tìm SSN có định dạng mạnh trước năm 2011 được định dạng bằng dấu gạch ngang hoặc dấu cách (ddd-dd-dddd HOẶC ddd dddd)

  - Func_unformatted_ssn sẽ tìm SSN có định dạng mạnh trước năm 2011 không được định dạng là chín chữ số liên tiếp (dddddddd)

  - Func_randomized_formatted_ssn sẽ tìm SSN sau năm 2011 được định dạng bằng dấu gạch ngang hoặc dấu cách (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn sẽ tìm SSN sau năm 2011 không được định dạng là chín chữ số liên tiếp (dddddddd)

- **[Kiểm tra:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Không, không có Checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Chính sách DLP tự tin rằng nó đã phát hiện ra loại thông tin nhạy cảm này nếu nằm trong khoảng cách 300 ký tự:

  - Hàm [sẽ Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nội dung khớp với mẫu hình.

  - Tìm thấy một [từ Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) từ khóa. Ví dụ về từ khóa bao gồm:  *An sinh Xã hội, An sinh Xã hội#, Sec Soc ,SSN*  . Ví dụ: mẫu sau đây sẽ kích hoạt cho chính sách DLP SSN: **SSN: 489-36-8350**
  
Để biết thêm thông tin về những gì cần thiết để phát hiện SSN cho nội dung của bạn, hãy xem phần sau trong bài viết này: Kiểu Thông tin Nhạy cảm sẽ trông như thế nào cho [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Dùng một kiểu thông tin nhạy cảm khác nhau, hãy xem bài viết sau đây để biết thông tin về những gì được yêu cầu cho các kiểu khác: Kiểu Thông tin Nhạy cảm [sẽ tìm kiếm điều gì](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  