---
title: Quy tắc cho số tài khoản ngân hàng Hoa Kỳ không hoạt động
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679318"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Các vấn đề về các số tài khoản ngân hàng Hoa Kỳ

**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Các vấn đề về các số tài khoản ngân hàng Hoa Kỳ**

Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung có chứa một **số tài khoản ngân hàng Hoa Kỳ** khi sử dụng kiểu thông tin nhạy cảm trong O365? Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với một chính sách **số tài khoản ngân hàng Hoa Kỳ** với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 chữ số

- **[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 chữ số liên tiếp.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Chính sách có thể là 75% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Biểu thức thông thường Regex_usa_bank_account_number tìm nội dung khớp với mẫu

  - Tìm thấy một từ khóa từ Keyword_usa_Bank_Account.

    Ví dụ, mẫu sau đây sẽ kích hoạt cho chính sách **số tài khoản ngân hàng Hoa Kỳ** : kiểm tra tài khoản 78344011

Để biết thêm thông tin về những điều cần thiết đối với **số tài khoản ngân hàng Hoa Kỳ** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm nào tìm kiếm số tài khoản ngân hàng Hoa Kỳ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  