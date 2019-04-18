---
title: Xác định địa chỉ IP và các khách hàng trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909683"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Xác định địa chỉ IP và các khách hàng trong Nhật ký kiểm tra

Địa chỉ IP tương ứng với một hoạt động của một người dùng hay quản trị được thể hiện trong Nhật ký kiểm tra. Thông tin khách hàng cũng đã đăng nhập. Dưới đây là các bước để xác định các thông tin như vậy

1. Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)

2. Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.

   Nếu bạn đang quan tâm đến một hoạt động cụ thể, chọn nó từ danh sách **các hoạt động** . Nếu không, tất cả các hoạt động sẽ được trả lại cho người dùng lựa chọn (cài đặt mặc định).

   **Lưu ý**: một số hoạt động có thể không có sẵn trong menu **hoạt động** ; Tuy nhiên, những người kiểm toán khoản mục này sẽ được trả lại nếu **Hiển thị kết quả cho tất cả các hoạt động** là lựa chọn (cài đặt mặc định).

3. Chỉ định tên người dùng trong lĩnh vực **người dùng** , chọn phạm vi ngày thích hợp cho các hoạt động, và sau đó nhấp vào **Tìm kiếm**.

Trong kết quả, bạn có thể xem địa chỉ IP cho rằng hoạt động trong ngăn kết quả. Chọn hồ sơ kiểm toán để xem thông tin chi tiết tại flyout **thông tin chi tiết** (ví dụ, khách hàng, người sử dụng thực hiện hành động, vv).

Để biết thêm chi tiết, hãy xem [Tìm địa chỉ IP của máy tính được sử dụng để truy cập vào một tài khoản bị xâm phạm](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
