---
title: Giảm thiểu Lỗi không phát hiện được ứng dụng
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
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026136"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Giảm thiểu lỗi "Không phát hiện thấy ứng dụng"

Lỗi cài đặt ứng dụng "Ứng dụng không được phát hiện sau khi hoàn tất cài đặt thành công", được Intune báo cáo, có thể xảy ra trên tất cả các nền tảng HĐH chính (Windows, iOS và Android).

Các kịch bản phổ biến nhất tạo ra lỗi này bao gồm:

- Ứng dụng đã được cập nhật bên ngoài Intune (từ cửa hàng ứng dụng của bên thứ ba) sau khi triển khai ban đầu. Ví dụ: một số ứng dụng như Google Chrome có thể thực hiện cập nhật tự động.
- Người dùng đã gỡ cài đặt ứng dụng sau lần cài đặt đầu tiên.

Để giảm thiểu sự cố này, trước tiên hãy thực hiện xem xét các thiết bị ảnh hưởng để xác định kịch bản xảy ra lỗi.

- Nếu ứng dụng đã được cập nhật bên ngoài Intune, triển khai ứng dụng có thể được đặt để bỏ qua phiên bản ứng dụng. Để làm như vậy, trong **Cấu hình Ứng dụng > Thông tin Ứng dụng**, hãy đặt Bỏ qua **phiên** bản Ứng dụng **thành Có.**
- Khi hướng tới máy khách, việc triển khai ứng dụng dưới dạng "bắt buộc" có thể phù hợp và đảm bảo rằng phiên bản mới nhất được triển khai.
- Ngoài ra, trên nền tảng iOS, bạn có thể sử dụng chức năng **tự** động cập nhật liên kết với Chương trình Mua Hàng Lớn của Apple, chương trình này có thể được đặt cấu hình để tự động cập nhật lên phiên bản ứng dụng mới khi chúng sẵn dùng.

Để biết thêm thông tin về cách khắc phục sự cố cài đặt ứng dụng, vui lòng xem Khắc [phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/intune/troubleshoot-app-install).
