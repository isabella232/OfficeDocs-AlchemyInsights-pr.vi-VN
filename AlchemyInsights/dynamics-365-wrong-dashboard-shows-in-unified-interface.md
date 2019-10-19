---
title: Dynamics 365-bảng điều khiển hiển thị sai trong Dynamics 365 giao diện hợp nhất
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528573"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Bảng điều khiển không đúng Hiển thị trong Dynamics 365 giao diện hợp nhất

Có một số lý do khiến bạn có thể thấy một bảng thông tin khác với trang bạn mong muốn:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Người dùng đã đặt bảng điều khiển mặc định của người dùng 

Thông thường, bạn có thể xác định một bảng điều khiển mặc định người dùng được thiết lập nếu nút **đặt làm mặc định** không hiển thị trong thanh lệnh bảng điều khiển. Bảng điều khiển mặc định người dùng sẽ ghi đè tất cả các bảng thông tin mặc định khác, ngay cả khi bảng điều khiển mặc định của người dùng không có trong ứng dụng hiện tại.

Sử dụng giải pháp sau để unset bảng điều khiển mặc định của họ.

1. Tạo bảng thông tin cá nhân mới.

2. Đặt bảng thông tin mới là mặc định của người dùng.

3. Xóa bảng thông tin đó.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Bảng điều khiển được đặt trong sơ đồ trang web

Bạn có thể đã đặt một bảng điều khiển mặc định của tổ chức bằng cách chọn một bảng thông tin và chọn ' đặt làm mặc định ' trong ' tùy chỉnh hệ thống '. Tuy nhiên, bảng điều khiển được xác định trong thiết kế sơ đồ trang web sẽ được ưu tiên hơn bảng điều khiển này, nếu người dùng có quyền truy cập vào nó.

Để có người dùng xem bảng thông tin bạn đã đặt làm mặc định của tổ chức, bạn có thể:

* Đặt bảng thông tin đó trong sơ đồ trang web

* Xóa quyền truy cập vào bảng điều khiển được xác định bởi Sơ đồ trang web cho những người dùng đó
