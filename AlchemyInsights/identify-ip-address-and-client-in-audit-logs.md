---
title: Xác định địa chỉ IP và máy khách trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668332"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Xác định địa chỉ IP và máy khách trong Nhật ký kiểm tra

Địa chỉ IP tương ứng với một hoạt động bởi một người dùng Microsoft 365 hoặc người quản trị được hiển thị trong Nhật ký kiểm tra. Thông tin máy khách cũng được ghi nhật ký. Sau đây là các bước để xác định thông tin đó

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).

2. Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.

   Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn nó từ danh sách **hoạt động** . Nếu không, tất cả các hoạt động sẽ được trả về cho người dùng được chọn (thiết đặt mặc định).

   **Lưu ý**: một số hoạt động có thể không sẵn dùng trong menu **hoạt động** ; Tuy nhiên, những mục kiểm tra này sẽ được trả về nếu **Hiển thị kết quả cho tất cả các hoạt động** được chọn (thiết đặt mặc định).

3. Xác định tên người dùng trong trường **người dùng** , chọn phạm vi ngày thích hợp cho hoạt động rồi sau đó bấm **Tìm kiếm**.

Trong kết quả, bạn có thể thấy địa chỉ IP cho hoạt động đó trong ngăn kết quả. Chọn bản ghi kiểm tra để xem thông tin chi tiết trong các **chi tiết** đã phát ra (ví dụ, máy khách, người dùng thực hiện hành động, v.v.).

Để biết thêm thông tin, hãy xem [Tìm địa chỉ IP của máy tính được dùng để truy nhập vào tài khoản bị xâm](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)phạm.
