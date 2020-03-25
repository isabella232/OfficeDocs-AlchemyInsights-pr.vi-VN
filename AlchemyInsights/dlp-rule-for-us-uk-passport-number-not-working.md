---
title: Quy tắc DLP cho US/UK Passport Number không làm việc
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931284"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Vấn đề với DLP-US/Vương Quốc Anh số hộ chiếu

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

**Các vấn đề DLP với số hộ chiếu Mỹ/Anh**

Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số hộ chiếu Mỹ/Anh** khi sử dụng một loại thông tin nhạy cảm DLP trong O365? Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với một chính sách **số hộ chiếu Mỹ/Anh** được cấu hình với mức độ tin cậy 75%, sau đây là đánh giá và phải được phát hiện cho quy tắc kích hoạt
  
- **[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Chín chữ số

- **[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Chín số liên tiếp

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Chức năng Func_usa_uk_passport tìm thấy nội dung phù hợp với mẫu.

  - Một từ khóa từ Keyword_passport được tìm thấy.

    Ví dụ, mẫu sau đây kích hoạt cho **Hoa Kỳ/anh số hộ chiếu** chính sách: US passport Number 123456789

Để biết thêm thông tin về những gì được yêu cầu đối với một số hộ chiếu Mỹ/Anh được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm số hộ chiếu Hoa Kỳ/Vương Quốc Anh](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  