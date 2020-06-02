---
title: Quy tắc DLP cho US/UK Passport Number không làm việc
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507320"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Vấn đề với DLP-US/Vương Quốc Anh số hộ chiếu

**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**Các vấn đề DLP với số hộ chiếu Mỹ/Anh**

Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số hộ chiếu Mỹ/Anh** khi sử dụng một loại thông tin nhạy cảm DLP trong O365? Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.
  
Ví dụ: đối với một chính sách **số hộ chiếu Mỹ/Anh** được cấu hình với mức độ tin cậy 75%, sau đây là đánh giá và phải được phát hiện cho quy tắc kích hoạt
  
- **[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Chín chữ số

- **[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Chín số liên tiếp

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum

- **[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:

  - Chức năng Func_usa_uk_passport tìm thấy nội dung phù hợp với mẫu.

  - Một từ khóa từ Keyword_passport được tìm thấy.

    Ví dụ, mẫu sau đây kích hoạt cho **Hoa Kỳ/anh số hộ chiếu** chính sách: US passport Number 123456789

Để biết thêm thông tin về những gì được yêu cầu đối với một số hộ chiếu Mỹ/Anh được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm số hộ chiếu Hoa Kỳ/Vương Quốc Anh](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  