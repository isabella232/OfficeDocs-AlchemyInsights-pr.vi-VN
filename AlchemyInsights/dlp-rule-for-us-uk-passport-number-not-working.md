---
title: Quy tắc DLP cho Số Hộ chiếu Hoa Kỳ/Vương quốc Anh không hoạt động
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004968"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Các vấn đề với DLP - số hộ chiếu Hoa Kỳ/Vương quốc Anh

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Các vấn đề về DLP với số hộ chiếu Hoa Kỳ/Vương quốc Anh**

Bạn đang gặp sự cố với tính năng Ngăn Mất Dữ liệu **(DLP)** không hoạt động đối với nội dung có chứa số hộ chiếu của Hoa **Kỳ/Vương** quốc Anh khi sử dụng kiểu thông tin nhạy cảm DLP trong O365? Nếu có, hãy đảm bảo nội dung của bạn chứa thông tin cần thiết cho thông tin cần thiết về những gì chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ, đối với chính sách số hộ chiếu của Hoa **Kỳ/Vương** quốc Anh được cấu hình với mức tin cậy 75%, các điều sau đây được đánh giá và phải được phát hiện để quy tắc kích hoạt
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Chín chữ số

- **[Mẫu hình:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Chín chữ số liên tiếp

- **[Kiểm tra:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có Checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Chính sách DLP tự tin rằng nó đã phát hiện ra loại thông tin nhạy cảm này nếu nằm trong khoảng cách 300 ký tự:

  - Hàm sẽ Func_usa_uk_passport nội dung khớp với mẫu hình.

  - Tìm thấy từ Keyword_passport từ khóa.

    Ví dụ, mẫu sau đây có thể kích hoạt cho chính sách số hộ chiếu của Hoa **Kỳ/Vương** quốc Anh: Số hộ chiếu Hoa 123456789

Để biết thêm thông tin về những gì cần thiết để phát hiện Số Hộ chiếu Hoa Kỳ/Vương quốc Anh để biết nội dung của bạn, hãy xem phần sau trong bài viết này: Kiểu Thông tin Nhạy cảm tìm Số Hộ chiếu Hoa [Kỳ/Vương](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) quốc Anh
  
Dùng một kiểu thông tin nhạy cảm khác nhau, hãy xem bài viết sau đây để biết thông tin về những gì được yêu cầu cho các kiểu khác: Kiểu Thông tin Nhạy cảm [sẽ tìm kiếm điều gì](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  