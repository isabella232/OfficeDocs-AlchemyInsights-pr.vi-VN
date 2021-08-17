---
title: Trợ giúp với cài đặt hiển thị ánh sáng đêm
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
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078752"
---
# <a name="help-with-the-night-light-display-setting"></a>Trợ giúp với cài đặt hiển thị ánh sáng đêm

Để tìm hiểu thêm về cài đặt hiển thị thời gian ban đêm, xem mục [Đặt hiển thị cho thời gian ban đêm Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Nếu tùy chọn ánh sáng đêm bị mờ trong màn hình Cài đặt, hãy kiểm tra trình điều khiển màn hình của bạn: 

1. Bấm vào hộp tìm kiếm trên thanh tác vụ của bạn và nhập **Trình quản lý Thiết bị**, sau đó chọn Trình quản lý Thiết **bị** trong kết quả tìm kiếm.
1. Bung **rộng Bộ điều hợp Hiển thị**. 

Rất tiếc, tính năng ánh sáng đêm không khả dụng nếu thiết bị của bạn sử dụng trình điều khiển DisplayLink hoặc trình điều khiển Màn hình Cơ bản.

Tính năng ánh sáng đêm sử dụng công nghệ đồ họa gần đây nên bạn có thể cần cập nhật trình điều khiển màn hình:  

- Kiểm tra bản cập nhật bằng cách đi **tới Bắt** đầu  >  **cập Cài đặt** Cập &  >  **Cập** Windows  >  **Cập nhật** Cập  >  **nhật**.  

HOẶC

- Truy nhập trang web hỗ trợ của nhà sản xuất phần cứng của bạn để tải xuống và cài đặt thủ công trình điều khiển hiển thị mới nhất.

## <a name="reset-night-light-in-the-registry"></a>Đặt lại ánh sáng đêm trong sổ đăng ký

Nếu việc cập nhật trình điều khiển màn hình không hoạt động, bạn có thể cần đặt lại ánh sáng đêm trong sổ đăng ký.  

**Thận trọng:** Bước khắc phục sự cố này chỉ được đề xuất cho người dùng nâng cao. Các sự cố nghiêm trọng có thể xảy ra nếu bạn sửa đổi sổ đăng ký không chính xác. Để bảo vệ tốt hơn, hãy sao lưu sổ đăng ký trước khi bạn sửa đổi để bạn có thể khôi phục nó nếu có vấn đề xảy ra.

1. Trong hộp tìm kiếm, nhập **regedit**, rồi chọn Trình soạn thảo **Sổ đăng ký** trong kết quả tìm kiếm.

1. Đi tới khóa sau của sổ đăng ký: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Xuất, rồi xóa khóa phụ sau đây:$$windows.data.bluelightreduction.bluelightreductionstate

1. Xuất, rồi xóa khóa phụ sau đây:$$windows.data.bluelightreduction.settings

1. Khởi động Windows lại và xác minh xem tùy chọn ánh sáng đêm có khả dụng không.


