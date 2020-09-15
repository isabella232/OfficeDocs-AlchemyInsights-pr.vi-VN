---
title: Quy tắc không hoạt động cho số hộ chiếu US/Vương Quốc Anh
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679246"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Các vấn đề với số lượng hộ chiếu US/UK

**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Phát sinh các vấn đề với số hộ chiếu US/Vương Quốc Anh**

Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung có chứa một **số hộ chiếu US/UK** khi sử dụng loại thông tin nhạy cảm trong O365? Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với một chính sách **số Passport US/UK** được cấu hình với mức độ tin cậy của 75%, các thao tác sau được đánh giá và phải được phát hiện cho quy tắc kích hoạt
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Chín chữ số

- **[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Chín chữ số liên tiếp

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Chính sách có thể là 75% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Hàm Func_usa_uk_passport tìm thấy nội dung khớp với mẫu.

  - Tìm thấy một từ khóa từ Keyword_passport.

    Ví dụ, mẫu sau đây sẽ kích hoạt cho chính sách **số hộ chiếu Hoa Kỳ/Vương Quốc Anh** : số hộ chiếu hoa kỳ 123456789

Để biết thêm thông tin về những điều cần thiết đối với số hộ chiếu US/UK sẽ được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm nào tìm kiếm đối với số hộ chiếu US/Vương Quốc Anh](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  