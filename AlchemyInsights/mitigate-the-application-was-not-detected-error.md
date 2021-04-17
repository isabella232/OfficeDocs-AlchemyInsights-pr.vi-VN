---
title: Giảm nhẹ ứng dụng không được phát hiện lỗi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836373"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Lỗi giảm thiểu "ứng dụng không được phát hiện"

Lỗi cài đặt ứng dụng, "ứng dụng không được phát hiện sau khi cài đặt đã hoàn tất thành công", được báo cáo bởi InTune, có thể xảy ra trên tất cả các nền tảng hệ điều hành chính (Windows, iOS và Android).

Các kịch bản phổ biến nhất tạo ra lỗi này bao gồm:

- Ứng dụng này đã được cập nhật bên ngoài InTune (từ App Store của bên thứ ba) sau khi triển khai ban đầu. Ví dụ một số ứng dụng chẳng hạn như Google Chrome có thể thực hiện cập nhật tự động.
- Người dùng đã gỡ cài đặt ứng dụng sau khi cài đặt ban đầu.

Để giảm thiểu sự cố này, trước tiên hãy thực hiện xem xét các thiết bị bị ảnh hưởng để xác định kịch bản có lỗi xảy ra.

- Nếu ứng dụng này đã được cập nhật bên ngoài InTune, triển khai ứng dụng có thể được thiết lập để bỏ qua phiên bản ứng dụng. Để thực hiện như vậy, bên dưới **thông tin ứng dụng cấu hình ứng dụng >**, hãy đặt **bỏ qua phiên bản ứng dụng** thành **có**.
- Khi mục tiêu của máy khách, có thể là phù hợp để triển khai ứng dụng là "bắt buộc" và để đảm bảo rằng phiên bản mới nhất được triển khai.
- Ngoài ra, trên nền tảng iOS, có thể sử dụng các chức năng **AutoUpdate** liên kết với chương trình mua âm lượng của Apple, có thể được cấu hình để tự động cập nhật các phiên bản ứng dụng mới khi chúng trở nên sẵn dùng.

Để biết thêm thông tin về khắc phục sự cố cài đặt ứng dụng, vui lòng xem [khắc phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/intune/troubleshoot-app-install).
