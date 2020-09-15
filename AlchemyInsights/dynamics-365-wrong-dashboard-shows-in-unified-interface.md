---
title: Dynamics 365-không hiển thị bảng điều khiển sai trong giao diện hợp nhất trong Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711297"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Không hiển thị bảng điều khiển sai trong giao diện hợp nhất trong Dynamics 365

Có một số lý do khiến bạn có thể thấy một bảng điều khiển khác với một bảng điều bạn mong đợi:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Người dùng đã thiết lập bảng điều khiển mặc định của người dùng 

Thông thường, bạn có thể xác định bảng điều khiển mặc định của người dùng được đặt nếu nút **đặt làm mặc định** không hiển thị trong thanh lệnh bảng điều khiển. Bảng điều khiển mặc định của người dùng sẽ ghi đè lên tất cả các bảng điều khiển mặc định khác, ngay cả khi bảng điều khiển mặc định của người dùng không có trong ứng dụng hiện tại.

Sử dụng giải pháp thay thế sau đây để bỏ đặt bảng điều khiển mặc định của họ.

1. Tạo bảng điều khiển cá nhân mới.

2. Đặt bảng điều khiển mới làm mặc định của người dùng.

3. Xóa bảng điều khiển đó.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Bảng điều khiển được đặt trong sơ đồ trang

Bạn có thể đã thiết lập một bảng điều khiển mặc định của tổ chức bằng cách chọn một bảng điều khiển và chọn ' đặt làm mặc định ' dưới ' tùy chỉnh hệ thống '. Nhưng bảng điều khiển được xác định trong trình thiết kế trang web sẽ được ưu tiên trên bảng điều khiển này, nếu người dùng có quyền truy nhập vào đó.

Để người dùng nhìn thấy bảng điều khiển bạn đã đặt làm mặc định của tổ chức, bạn có thể:

* Đặt bảng điều khiển đó trong sơ đồ trang

* Loại bỏ quyền truy nhập vào bảng điều khiển được xác định trong sitemap cho những người dùng đó
