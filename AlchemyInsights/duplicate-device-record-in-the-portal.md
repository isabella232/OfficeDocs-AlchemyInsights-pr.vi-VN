---
title: Bản ghi thiết bị trùng lặp trong cổng thông tin
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678526"
---
# <a name="duplicate-device-record-in-the-portal"></a>Bản ghi thiết bị trùng lặp trong cổng thông tin

Bạn có thể thấy 2 bản ghi cho một thiết bị trong cổng thông tin nếu thiết bị không chính xác báo cáo trạng thái quản lý đồng bộ với site trình quản lý cấu hình. Để kiểm tra trạng thái đồng quản lý của một thiết bị, hãy xem lại cột **đồng quản lý** cho thiết bị trong bảng điều khiển trình quản lý cấu hình. Nếu cột không hiển thị, bạn có thể thêm nó bằng cách bấm chuột phải vào bất kỳ tiêu đề cột nào, rồi chọn nó từ danh sách.

Giá trị đồng quản lý phải **có**. Nếu giá trị là **không**, hãy mở applet máy khách trình quản lý cấu hình trên thiết bị khách và kiểm tra thuộc tính **đồng quản lý** trong tab chung.

- Nếu giá trị được **bật**, điều này cho biết sự cố với giao tiếp khách hàng với điểm quản lý. Vui lòng xem **CcmMessaging. log** trên thiết bị để điều tra các vấn đề kết nối tiềm ẩn.

- Nếu giá trị bị **vô hiệu hóa** và thiết bị được đăng ký trong InTune, vui lòng đảm bảo rằng thiết bị đã nhận được chính sách đồng quản lý bằng cách xem lại **Comanagementhandler. đăng nhập** vào thiết bị.
