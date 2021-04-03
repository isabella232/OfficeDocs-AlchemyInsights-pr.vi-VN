---
title: Giải phóng dung lượng ổ đĩa trong Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505378"
---
# <a name="free-up-drive-space-in-windows-10"></a>Giải phóng dung lượng ổ đĩa trong Windows 10

Dưới đây là hai tùy chọn để giải phóng dung lượng ổ đĩa trong Windows:

- Giải phóng dung lượng ổ đĩa trong Windows 10.
- Giải phóng dung lượng cho các bản cập nhật Windows 10 với thiết bị lưu trữ bên ngoài.

Nếu bạn vẫn có dung lượng ổ đĩa thấp sau khi sử dụng dọn dẹp ổ đĩa, có thể là thư mục TEMP của bạn sẽ nhanh chóng được điền với các tệp ứng dụng (. appx) được Microsoft Store sử dụng. Để khắc phục sự cố này, hãy đặt lại cửa hàng, xóa bộ đệm ẩn lưu trữ, sau đó chạy trình khắc phục sự cố Windows Update. Đảm bảo rằng Microsoft Store sẽ được đóng lại trước khi bạn tiếp tục thực hiện các bước này.

**Bước 1: đặt lại Microsoft Store**

**Ghi chú** Việc này sẽ xóa vĩnh viễn dữ liệu ứng dụng trên thiết bị, bao gồm các tùy chọn và chi tiết đăng nhập của bạn.

1. Chọn thiết đặt **bắt đầu** ứng dụng  >    >  **ứng** dụng  >  **& các tính năng**.

1. Trong danh sách ứng dụng, định vị và chọn Microsoft Store.

1. Chọn **tùy chọn nâng cao**.

1. Cuộn xuống và chọn **đặt lại**, rồi **xác nhận đặt lại**.

**Bước 2: xóa bộ đệm ẩn Microsoft Store**

1. Nhấn phím logo Windows + R để mở hộp thoại chạy.

1. Nhập wsreset.exe và chọn **OK**.

1. Cửa sổ dấu nhắc lệnh trống mở ra. Sau khoảng 10 giây, cửa sổ sẽ đóng lại và cửa hàng mở ra tự động.

**Bước 3: đặt lại Windows Update**

1. Chọn **bắt đầu**  >    >  **Cập Nhật** cài đặt &  >  **khắc phục sự cố** bảo mật.

1. Cuộn xuống và chọn **Windows Update** từ danh sách, rồi chọn **chạy trình** khắc phục sự cố.

1. Khởi động lại máy tính của bạn và kiểm tra xem bạn vẫn đang gặp sự cố.

