---
title: Xác định địa chỉ IP và khách hàng trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508938"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Xác định địa chỉ IP và khách hàng trong Nhật ký kiểm tra

Địa chỉ IP tương ứng với một hoạt động của người dùng Microsoft 365 hoặc quản trị viên được hiển thị trong Nhật ký kiểm tra. Thông tin khách hàng cũng được ghi lại. Dưới đây là các bước để xác định thông tin đó

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).

2. Đi tới trang **Search**  >  **Tìm kiếm Nhật ký kiểm tra** tìm kiếm.

   Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn nó từ danh sách **hoạt động** . Nếu không, tất cả các hoạt động sẽ được trả lại cho người dùng đã chọn (cài đặt mặc định).

   **Lưu ý**: một số hoạt động có thể không có sẵn trong menu **hoạt động** ; Tuy nhiên, các mục kiểm tra sẽ được trả lại nếu **Hiển thị kết quả cho tất cả các hoạt động** được chọn (cài đặt mặc định).

3. Chỉ định tên người dùng trong trường **người sử dụng** , chọn phạm vi ngày thích hợp cho hoạt động, và sau đó bấm **Tìm kiếm**.

Trong kết quả, bạn có thể thấy địa chỉ IP cho hoạt động đó trong ngăn kết quả. Chọn bản ghi kiểm tra để xem thông tin chi tiết trong mục thả xuống **thông** tin (ví dụ: khách hàng, người dùng đã thực hiện hành động, v.v.).

Để biết thêm thông tin, hãy xem [Tìm địa chỉ IP của máy tính được sử dụng để truy cập tài khoản bị xâm phạm](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
