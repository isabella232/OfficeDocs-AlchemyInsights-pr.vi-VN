---
title: DLP quy tắc cho Hoa Kỳ / Vương Quốc Anh số hộ chiếu không làm việc
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28321228"
---
Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **U.S. / số hộ chiếu Anh Quốc** khi sử dụng một loại thông tin nhạy cảm DLP trong O365? Nếu vậy, hãy chắc chắn rằng nội dung của bạn sẽ chứa các thông tin cần thiết cho những gì chính sách DLP tìm kiếm khi nó được đánh giá. 
  
Ví dụ, cho một **U.S. / số hộ chiếu của Anh** chính sách được cấu hình với mức độ tin cậy của 75%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt 
  
- **[Định dạng:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 chữ số 
    
- **[Mẫu:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 chữ số liên tục 
    
- **[Kiểm tra:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, đó là không có kiểm tra 
    
- **[Định nghĩa:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Một chính sách DLP là 75% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự: 
    
  - Chức năng Func_usa_uk_passport tìm thấy nội dung phù hợp với các mô hình.
    
  - Tìm thấy một từ khóa từ Keyword_passport.
    
    Ví dụ, các mẫu sau sẽ kích hoạt cho các **U.S. / số hộ chiếu Anh Quốc** sách: hộ chiếu Hoa Kỳ số 123456789 
    
Để biết thêm về những gì là cần thiết cho một Mỹ / số hộ chiếu Anh Quốc để được phát hiện cho nội dung của bạn, xem phần sau đây trong bài viết này: [xem xét những gì the nhạy cảm thông tin loại cho Hoa Kỳ / số hộ chiếu Anh Quốc](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

