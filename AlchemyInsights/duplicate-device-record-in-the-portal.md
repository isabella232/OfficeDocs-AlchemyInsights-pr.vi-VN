---
title: Bản ghi thiết bị trùng lặp trong cổng thông tin
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790179"
---
# <a name="duplicate-device-record-in-the-portal"></a>Bản ghi thiết bị trùng lặp trong cổng thông tin

Bạn có thể thấy 2 hồ sơ cho một thiết bị trong cổng nếu thiết bị không đúng cách báo cáo trạng thái đồng quản lý trang web quản lý cấu hình. Để kiểm tra tình trạng đồng quản lý của thiết bị, xem cột **đồng quản lý** thiết bị trong bảng điều khiển quản lý cấu hình. Nếu cột không hiển thị, bạn có thể thêm nó bằng cách bấm chuột phải vào bất kỳ tiêu đề cột nào và chọn nó từ danh sách.

Giá trị đồng quản lý phải **có**. Nếu giá trị là **không**, mở cấu hình quản lý khách hàng applet trên thiết bị khách hàng và kiểm tra thuộc tính **đồng quản lý** trong tab chung.

- Nếu giá trị được **kích hoạt**, điều này cho biết vấn đề với giao tiếp khách hàng quản lý điểm. Vui lòng đánh giá **Ccmmessaging. log** trên thiết bị để điều tra vấn đề kết nối tiềm năng.

- Nếu giá trị bị **vô hiệu hoá** và thiết bị được đăng ký trong InTune, hãy đảm bảo rằng thiết bị đã nhận được chính sách đồng quản lý bằng cách xem **Comanagementhandler. log** trên thiết bị.
