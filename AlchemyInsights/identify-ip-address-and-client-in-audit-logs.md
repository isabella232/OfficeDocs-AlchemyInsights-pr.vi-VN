---
title: Xác định địa chỉ IP và máy khách trong nhật ký kiểm tra
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
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887522"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Xác định địa chỉ IP và máy khách trong nhật ký kiểm tra

Địa chỉ IP tương ứng với một hoạt động do người dùng hoặc người quản Microsoft 365 của họ thực hiện được hiển thị trong Nhật ký Kiểm tra. Thông tin máy khách cũng được ghi nhật ký. Dưới đây là các bước để xác định thông tin đó

1. Đăng nhập vào Trung [tâm Microsoft 365 Tuân thủ .](https://protection.office.com/)

2. Đi đến trang Tìm **kiếm nhật** ký  >  **kiểm tra.**

   Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn hoạt động đó từ danh **sách Hoạt** động. Nếu không, tất cả các hoạt động sẽ được trả về cho người dùng đã chọn (cài đặt mặc định).

   **Lưu ý:** Một số hoạt động nhất định có thể không sẵn dùng trong menu **Hoạt** động; tuy nhiên, các mục kiểm tra này sẽ được trả về nếu mục **Hiển thị Kết quả cho tất cả các hoạt** động được chọn (cài đặt mặc định).

3. Chỉ định tên người dùng trong **trường Người** dùng, chọn phạm vi ngày thích hợp cho hoạt động, rồi bấm Tìm **kiếm.**

Trong kết quả, bạn có thể thấy địa chỉ IP của hoạt động đó trong ngăn kết quả. Chọn bản ghi kiểm tra  để xem thông tin chi tiết trong hộp bật lên Chi tiết (ví dụ: Máy khách, Người dùng đã thực hiện hành động, v.v.).

Để biết thêm thông tin, hãy [xem Tìm địa chỉ IP của máy tính được dùng để truy nhập tài khoản bị xâm phạm.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
