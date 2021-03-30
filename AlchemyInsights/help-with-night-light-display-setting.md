---
title: Trợ giúp với thiết đặt hiển thị ánh sáng đêm
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
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405186"
---
# <a name="help-with-the-night-light-display-setting"></a>Trợ giúp với thiết đặt hiển thị ánh sáng đêm

Để tìm hiểu thêm về thiết đặt hiển thị thời gian ban đêm, hãy xem [thiết đặt màn hình hiển thị của bạn cho thời gian ban đêm trong Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Nếu các tùy chọn ánh sáng ban đêm được tô xám trong thiết đặt, hãy kiểm tra trình điều khiển hiển thị của bạn: 

1. Bấm vào hộp tìm kiếm trên thanh tác vụ và nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** trong kết quả tìm kiếm.
1. Bung rộng bộ điều hợp **Hiển thị**. 

Rất tiếc, tính năng đêm chiếu sáng không sẵn dùng nếu thiết bị của bạn sử dụng trình điều khiển DisplayLink hoặc trình điều khiển hiển thị cơ bản.

Tính năng chiếu sáng ban đêm làm cho việc sử dụng công nghệ đồ họa gần đây, vì vậy bạn có thể cần cập nhật trình điều khiển hiển thị của mình:  

- Kiểm tra các bản Cập Nhật bằng cách đi đến **bắt đầu**  >  Cập Nhật **cài đặt**  >  **& bảo mật**  >  **Windows Update**  >  **kiểm tra Cập Nhật**.  

HAY

- Truy nhập trang web hỗ trợ của nhà sản xuất phần cứng để tải xuống theo cách thủ công và cài đặt trình điều khiển hiển thị mới nhất.

## <a name="reset-night-light-in-the-registry"></a>Đặt lại ánh sáng đêm trong sổ đăng ký

Nếu Cập Nhật trình điều khiển hiển thị của bạn không hoạt động, bạn có thể cần đặt lại ánh sáng đêm trong sổ đăng ký.  

**Thận trọng:** Bước khắc phục sự cố này chỉ được đề xuất dành cho người dùng nâng cao. Các vấn đề nghiêm trọng có thể xảy ra nếu bạn sửa đổi không chính xác của sổ đăng ký. Để được thêm bảo vệ, hãy sao lưu sổ đăng ký trước khi bạn sửa đổi để bạn có thể khôi phục nó nếu vấn đề xảy ra.

1. Trong hộp tìm kiếm, nhập **regedit**, rồi chọn **trình soạn thảo sổ đăng ký** trong kết quả tìm kiếm.

1. Đi đến khóa đăng ký sau đây: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Xuất và sau đó xóa khóa phụ sau đây: $ $windows. Data. bluelightreduction. bluelightreductionstate

1. Xuất và sau đó xóa khóa phụ sau đây: $ $windows. Data. bluelightreduction. Settings

1. Khởi động lại Windows và xác nhận xem tùy chọn ánh sáng đêm sẵn dùng.


