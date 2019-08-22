---
title: Dynamics 365 - bảng điều khiển sai cho thấy trong giao diện thống nhất Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528573"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Bảng điều khiển sai cho thấy trong giao diện thống nhất Dynamics 365

Có rất nhiều lý do tại sao bạn có thể thấy một bảng điều khiển khác nhau hơn bạn mong đợi:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Người dùng đã thiết lập một bảng điều khiển người dùng mặc định 

Thông thường bạn có thể xác định một người sử dụng bảng điều khiển mặc định được thiết lập nếu nút **Đặt làm mặc định** không hiển thị trong bảng điều khiển lệnh thanh. Người dùng mặc định bảng sẽ ghi đè lên tất cả các mặc định trang tổng quan, thậm chí nếu người dùng mặc định bảng điều khiển không phải là các ứng dụng hiện tại.

Sử dụng các workaround sau đây để bỏ đặt của bảng điều khiển mặc định.

1. Tạo ra một bảng điều khiển cá nhân mới.

2. Đặt rằng bảng điều khiển mới như mặc định của người dùng.

3. Xóa bảng đó.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Bảng điều khiển được đặt trong sơ đồ trang web

Bạn có thể đã thiết lập một tổ chức mặc định bảng bằng cách chọn một bảng điều khiển và chọn 'Thiết lập như mặc định' dưới 'Tùy chỉnh các hệ thống'. Nhưng bảng điều khiển được định nghĩa trong các thiết kế sơ đồ trang web sẽ được ưu tiên qua bảng điều khiển này, nếu người dùng có quyền truy cập vào nó.

Để người dùng xem các bảng điều khiển bạn đã thiết lập mặc định của tổ chức, bạn có thể:

* Đặt rằng bảng điều khiển trong sơ đồ trang web

* Loại bỏ quyền truy cập vào bảng sơ đồ trang web xác định cho những người dùng
