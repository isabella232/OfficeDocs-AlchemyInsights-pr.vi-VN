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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902282"
---
# <a name="find-the-ip-address-in-audit-log"></a>Tìm địa chỉ IP trong nhật ký kiểm tra

Địa chỉ IP tương ứng với hoạt động được thực hiện bởi người dùng hoặc người quản trị được hiển thị trong nhật ký kiểm tra. Thông tin máy khách cũng được ghi nhật ký. Dưới đây là cách xác định địa chỉ IP:

1. Thực hiện một trong các thao tác sau:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. If this feature isn't enabled, search results won't be able to pull data from previous dates.

2. On the **Audit** page, verify that the **Search** tab is selected and then configure the following settings:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt** động: Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn hoạt động đó từ danh sách; nếu không, giá trị mặc định **Hiển thị kết quả cho tất cả các hoạt** động sẽ trả về tất cả các hoạt động.. Lưu ý rằng một số hoạt động nhất định có thể không sẵn dùng để lựa chọn; tuy nhiên, các mục kiểm tra này sẽ được trả về nếu **mục Hiển thị kết quả cho tất cả các hoạt** động được chọn.
   - **Người dùng:** Chấp nhận giá trị mặc định trống để trả về kết quả cho tất cả người dùng hoặc nhập một hoặc nhiều người dùng.

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Trong kết quả, bấm vào **Lọc Kết quả,** **rồi nhập Set-Mailbox** vào hộp bộ lọc hoạt động.

5. Chọn một bản ghi kiểm tra trong kết quả để mở hộp **bật lên** Chi tiết.

Để biết thêm thông tin, hãy xem [Tìm kiếm nhật ký kiểm tra để điều tra các sự cố hỗ trợ phổ biến.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
