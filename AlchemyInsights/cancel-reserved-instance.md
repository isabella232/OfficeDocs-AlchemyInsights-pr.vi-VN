---
title: Hủy bỏ Đặt trước
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931255"
---
# <a name="cancelling-reservation"></a>Hủy bỏ Đặt trước

- **Tự phục vụ:** Bạn có thể tự hủy hoặc đổi phiên bản dành riêng bằng cổng [thông tin Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Chọn đặt trước, rồi bấm vào hoàn tiền hoặc đổi lại. Lưu ý rằng bạn phải có quyền truy cập chủ sở hữu trên Lệnh Đặt trước để đổi lại hoặc hoàn tiền. Việc truy cập vào chỉ Đặt trước sẽ không cho phép bạn tiếp tục hoàn tiền hoặc đổi lại. Yêu cầu chủ sở hữu Yêu cầu Đặt trước cung cấp cho bạn quyền truy cập của chủ sở hữu vào Lệnh Đặt trước
- **Exchange sách mới:** Bạn có thể trao đổi đặt trước để giữ lại một loại đặt trước khác – không có **hình thức trừng phạt nào** đối với việc trao đổi đặt trước. Tổng cam kết với việc đặt trước mới phải lớn hơn tổng số tiền hoàn lại cho việc đặt trước đã trao đổi và các khoản thanh toán hàng tháng trong tương lai (nếu có)
- **Chính sách hoàn tiền:** Tổng tiền hoàn trả và các khoản thanh toán trong tương lai đã hủy bỏ không được vượt quá $50.000 USD trong một cửa sổ liên kết 12 tháng. Hiện tại, **chúng tôi không tính bất kỳ khoản tiền hoàn lại nào** cho việc hoàn tiền nhưng có thể tính phí cho các khoản hoàn tiền trong tương lai  
    **Ngoại lệ:** Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp hàng
- **Api / PS / CLI** không sẵn có để hủy bỏ và hoàn tiền cho trao đổi tự phục vụ và hoàn tiền cho Việc đặt trước [Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp khách hàng. Hỗ trợ các loại đăng ký khác của Chính phủ Hoa Kỳ bao gồm Thanh toán Khi Di chuyển và CSP

Tìm hiểu thêm: [Cách xử lý các giao dịch trả lại và trao đổi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Tìm hiểu thêm : Chính [Exchange và Hoàn tiền](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Câu hỏi khác: [Truy cập tài liệu phiên bản dành riêng](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange một phiên bản dành riêng hiện có (Tự phục vụ)**

Bạn có thể đổi phần bảo lưu cho một phần bảo lưu khác có cùng loại. Bạn cũng có thể hoàn tiền cho việc đặt trước, tối đa $50.000 USD mỗi năm, nếu bạn không cần nữa. Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp khách hàng. Hỗ trợ các loại đăng ký khác của Chính phủ Hoa Kỳ, bao gồm Thanh toán Khi Di chuyển và CSP. Bạn phải có quyền truy cập của chủ sở hữu trên Lệnh Đặt trước để đổi lại hoặc hoàn lại tiền bảo lưu hiện có.

Các bước sau đây sẽ hướng dẫn quy trình hoàn tất giao dịch

1. Đăng nhập vào cổng thông [tin Azure của bạn.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Chọn mục đặt trước mà bạn muốn hoàn tiền và bấm vào **Exchange**
2. Chọn sản phẩm VM mà bạn muốn mua và nhập số lượng. Hãy đảm bảo rằng tổng mua hàng mới lớn hơn tổng hoàn vốn Xác định [kích cỡ phù hợp trước khi mua](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Xem lại và hoàn tất giao dịch

**Hoàn tiền cho bản thể hiện đã đặt trước**

Để hoàn tiền cho việc đặt trước, hãy đi tới Chi **tiết Đặt trước và** bấm vào Hoàn **tiền**

**Pro hoàn tiền được xếp hạng cao nhất:**

**Pro dụ về yêu cầu tối thiểu và hoàn tiền cho việc đổi trả**  
Ví dụ về đặt trước mặt trước:

- Bạn mua kỳ hạn một năm RI với giá $120 vào ngày 1 tháng 1
- Vào 07 Tháng Tư, bạn muốn hoàn tiền hoặc đổi thông tin đặt trước này
- Vì đặt trước đã hoạt động trong 97 ngày, bạn sẽ nhận được (1-97/365) * $120 trở lại. (tức là $88,1). Hiện không có hình phạt nào đối với hoàn tiền
- Nếu trao đổi, giao dịch mua hàng mới của bạn phải lớn hơn $88,1
- Hiện không có hình phạt nào đối với hoàn tiền

**Ví dụ về đặt trước gói thanh toán:**

- Bạn mua kỳ hạn một năm RI với giá $10 mỗi tháng
- Vào 07 Tháng Tư, bạn muốn hoàn tiền hoặc đổi thông tin đặt trước này
- Vì khoản thanh toán gần nhất đã diễn ra 7 ngày, bạn sẽ nhận được (1-7/31) * $10 trở lại. (ví dụ: $7,74)
- Các khoản thanh toán trong tương lai đã bị hủy bỏ là $ 80. Hiện không có hình phạt nào đối với hoàn tiền
- Hủy bỏ này sẽ trừ $87,74 khỏi giới hạn hoàn tiền $50.000
- Nếu trao đổi, tổng giá trị của giao dịch mua hàng mới sẽ lớn hơn $87,74

**Tài liệu được Đề xuất**

- [Cách xử lý các giao dịch trả lại và trao đổi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange sách Hoàn tiền và Hoàn tiền](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)