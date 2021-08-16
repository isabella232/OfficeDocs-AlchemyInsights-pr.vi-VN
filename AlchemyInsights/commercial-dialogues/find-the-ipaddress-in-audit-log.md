---
title: Tìm địa chỉ IP trong nhật ký kiểm tra
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017154"
---
# <a name="find-the-ip-address-in-audit-log"></a>Tìm địa chỉ IP trong nhật ký kiểm tra

1. Địa chỉ IP tương ứng với hoạt động được thực hiện bởi người dùng hoặc người quản trị được hiển thị trong nhật ký kiểm tra. Thông tin máy khách cũng được ghi nhật ký. Dưới đây là cách xác định địa chỉ IP:

1. Đi đến Trung [tâm Office 365 chính sách Bảo & Tuân thủ](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Chọn Tìm **kiếm Tìm** kiếm Nhật ký  >  **[kiểm tra](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. If this feature isn't enabled, search results won't be able to pull data from previous dates.
1. Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn hoạt động đó từ danh **sách Hoạt** động; nếu không, theo mặc định, tất cả các hoạt động sẽ được trả về cho người dùng đã chọn. Lưu ý rằng một số hoạt động nhất định có thể không sẵn dùng để lựa chọn từ menu **Hoạt** động; tuy nhiên, các mục kiểm tra này sẽ được trả về nếu mục **Hiển thị kết quả cho tất cả các hoạt** động được chọn (cài đặt mặc định).
1. Xác định phạm vi ngày và trong trường **Người dùng,** chọn tên người dùng cho người dùng bạn muốn điều tra.
1. Chọn **Tìm kiếm**. Các hoạt động xuất hiện bên dưới **Kết quả**. Bạn có thể thấy địa chỉ IP cho từng hoạt động.
1. Để xem chi tiết, hãy chọn một hoạt động, rồi chọn Xem **thêm Thông tin**.

Để tìm hiểu thêm, xem mục Tìm kiếm nhật [Office 365 kiểm tra để khắc phục các tình huống phổ biến.](https://go.microsoft.com/fwlink/?linkid=2103944)