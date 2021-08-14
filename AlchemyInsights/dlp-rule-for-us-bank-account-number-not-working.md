---
title: Quy tắc DLP cho Số Tài khoản Ngân hàng Hoa Kỳ không hoạt động
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005040"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Sự cố DLP với số tài khoản ngân hàng tại Hoa Kỳ

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Sự cố DLP với số tài khoản ngân hàng tại Hoa Kỳ**

Bạn đang gặp sự cố với tính năng Ngăn  Mất Dữ liệu **(DLP)** không hoạt động đối với nội dung có chứa Số Tài khoản Ngân hàng Hoa Kỳ khi sử dụng kiểu thông tin nhạy cảm DLP trong O365? Nếu có, hãy đảm bảo nội dung của bạn chứa thông tin cần thiết cho thông tin cần thiết về những gì chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ,  đối với chính sách Số Tài khoản Ngân hàng Hoa Kỳ được cấu hình với mức tin cậy là 85%, những điều sau đây được đánh giá và phải được phát hiện để quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 chữ số

- **[Mẫu hình:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 chữ số liên tiếp.

- **[Kiểm tra:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có Checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Chính sách DLP tự tin rằng nó đã phát hiện ra loại thông tin nhạy cảm này nếu nằm trong khoảng cách 300 ký tự:

  - Biểu thức thông thường Regex_usa_bank_account_number thấy nội dung phù hợp với mẫu hình

  - Tìm thấy từ Keyword_usa_Bank_Account từ khóa.

    Ví dụ: mẫu sau đây sẽ kích hoạt cho chính sách Số Tài **khoản Ngân hàng** Hoa Kỳ: Kiểm tra Tài khoản 78344011

Để biết thêm thông tin  về những gì bắt buộc để Số Tài khoản Ngân hàng Hoa Kỳ được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: Kiểu Thông tin Nhạy cảm sẽ tìm số Tài khoản Ngân hàng Hoa [Kỳ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Dùng một kiểu thông tin nhạy cảm khác nhau, hãy xem bài viết sau đây để biết thông tin về những gì được yêu cầu cho các kiểu khác: Kiểu Thông tin Nhạy cảm [sẽ tìm kiếm điều gì](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  