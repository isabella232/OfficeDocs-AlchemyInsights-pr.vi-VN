---
title: Bản ghi thiết bị trùng lặp trong cổng thông tin
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
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004176"
---
# <a name="duplicate-device-record-in-the-portal"></a>Bản ghi thiết bị trùng lặp trong cổng thông tin

Bạn có thể thấy 2 bản ghi cho một thiết bị trong cổng thông tin nếu thiết bị đó không báo cáo chính xác trạng thái đồng quản lý cho site Trình quản lý Cấu hình. Để kiểm tra trạng thái đồng quản lý của thiết bị, hãy xem lại **cột Đồng** được quản lý cho thiết bị trong bảng điều khiển Trình quản lý Cấu hình. Nếu cột không hiển thị, bạn có thể thêm nó bằng cách bấm chuột phải vào bất kỳ tiêu đề cột nào và chọn nó từ danh sách.

Giá trị Đồng quản lý phải là **Có.** Nếu giá trị là **Không,** hãy mở applet máy khách Trình quản lý Cấu hình trên thiết bị khách và kiểm tra thuộc tính **Đồng** quản lý trong tab Chung.

- Nếu giá trị đó được Bật , **điều này cho** biết các vấn đề liên lạc với máy khách với Điểm Quản lý. Vui lòng xem lại **CcmMessaging.log trên thiết bị để** điều tra các sự cố kết nối tiềm ẩn.

- Nếu giá  trị là Bị vô hiệu hóa và thiết bị được đăng ký trong Intune, vui lòng đảm bảo rằng thiết bị đã nhận được chính sách Đồng quản lý bằng cách xem **lại CoManagementHandler.log** trên thiết bị.
