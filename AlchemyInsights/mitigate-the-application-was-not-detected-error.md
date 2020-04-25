---
title: Giảm thiểu các ứng dụng không được phát hiện lỗi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810505"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Giảm thiểu lỗi "ứng dụng không được phát hiện"

Lỗi cài đặt ứng dụng, "ứng dụng không được phát hiện sau khi cài đặt hoàn tất thành công," báo cáo của InTune, có thể xảy ra trên tất cả các nền tảng hệ điều hành chính (Windows, iOS và Android).

Các trường hợp phổ biến nhất tạo ra lỗi này bao gồm:

- Ứng dụng đã được cập nhật bên ngoài InTune (từ cửa hàng ứng dụng của bên thứ ba) sau khi triển khai ban đầu. Ví dụ một số ứng dụng như Google Chrome có thể thực hiện cập nhật tự động.
- Một người dùng đã gỡ cài đặt các ứng dụng sau khi cài đặt ban đầu.

Để giảm thiểu vấn đề này, đầu tiên thực hiện đánh giá các thiết bị bị ảnh hưởng để xác định tình huống trong đó lỗi xảy ra.

- Nếu ứng dụng đã được cập nhật bên ngoài InTune, việc triển khai ứng dụng có thể được đặt để bỏ qua phiên bản ứng dụng. Để làm như vậy, trong **ứng dụng cấu hình > thông tin ứng dụng**, thiết lập **bỏ qua phiên bản ứng dụng** **có**.
- Khi nhắm mục tiêu khách hàng, có thể thích hợp để triển khai ứng dụng là "bắt buộc" và để đảm bảo rằng phiên bản mới nhất được triển khai.
- Ngoài ra, trên nền tảng iOS, có thể sử dụng chức năng **AutoUpdate** liên quan đến chương trình mua ổ đĩa của Apple, có thể được cấu hình để tự động cập nhật phiên bản ứng dụng mới khi chúng trở nên có sẵn.

Để biết thêm thông tin về khắc phục sự cố cài đặt ứng dụng, vui lòng xem [khắc phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/intune/troubleshoot-app-install).
