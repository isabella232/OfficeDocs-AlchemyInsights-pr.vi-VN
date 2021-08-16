---
title: Dynamics 365 - Hiển thị Sai Bảng điều khiển trong Giao diện Hợp nhất Dynamics 365
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101504"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Bảng điều khiển hiển thị sai trong giao diện hợp nhất Dynamics 365

Có một số lý do tại sao bạn có thể thấy bảng điều khiển khác với bảng điều khiển bạn mong đợi:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Người dùng đã đặt một bảng điều khiển mặc định của người dùng 

Thông thường, bạn có thể xác định bảng thông tin mặc định của người dùng được đặt nếu nút Đặt **Làm** Mặc định không hiển thị trong thanh lệnh bảng điều khiển. Bảng điều khiển mặc định của người dùng sẽ ghi đè lên tất cả các bảng điều khiển mặc định khác, ngay cả khi bảng điều khiển mặc định của người dùng không có trong ứng dụng hiện tại.

Sử dụng giải pháp thay thế sau đây để bỏ đặt bảng điều khiển mặc định của họ.

1. Tạo bảng điều khiển cá nhân mới.

2. Đặt bảng điều khiển mới đó làm mặc định cho người dùng.

3. Xóa bảng điều khiển đó.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Bảng điều khiển được đặt trong sơ đồ site

Bạn có thể đã đặt bảng điều khiển mặc định của tổ chức bằng cách chọn một bảng điều khiển và chọn 'Đặt Làm Mặc định' bên dưới 'Tùy chỉnh Hệ thống'. Nhưng bảng điều khiển được xác định trong trình thiết kế sơ đồ site sẽ được ưu tiên hơn bảng điều khiển này, nếu người dùng có quyền truy nhập vào đó.

Để cho phép người dùng nhìn thấy bảng điều khiển mà bạn đã đặt làm bảng điều khiển mặc định của tổ chức, bạn có thể:

* Đặt bảng điều khiển đó trong sơ đồ site

* Loại bỏ quyền truy nhập vào bảng điều khiển đã xác định của sơ đồ site cho những người dùng đó
