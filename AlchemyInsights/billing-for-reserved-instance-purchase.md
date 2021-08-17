---
title: Thanh toán cho giao dịch mua Phiên bản Dự phòng
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104042"
---
# <a name="billing-for-reserved-instance-purchase"></a>Thanh toán cho giao dịch mua Phiên bản Dự phòng

Giao dịch mua phiên bản bảo lưu được tính phí cho phương thức thanh toán gắn với đăng ký mà bạn chọn tại thời điểm mua. Loại đăng ký phải là thỏa thuận doanh nghiệp (số ưu đãi: MS-AZR-0017P), Pay-As-You-Go (số gói đăng ký: MS-AZR-0003P), Thỏa thuận Khách hàng của Microsoft hoặc CSP.

- Đối với đăng ký doanh nghiệp, phí được trừ khỏi số dư cam kết bằng tiền tệ của đăng ký hoặc bị tính phí quá hạn
- Đối với đăng ký Thanh toán Khi Bạn Sử dụng, các khoản phí sẽ được lập hóa đơn bằng thẻ tín dụng hoặc phương thức thanh toán hóa đơn trên đăng ký

**Hủy bỏ Đặt trước**

- **Tự phục vụ:** Bạn có thể tự hủy hoặc đổi phiên bản dành riêng bằng cổng [thông tin Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Chọn đặt trước, rồi bấm vào hoàn tiền hoặc đổi lại. Lưu ý rằng bạn phải có quyền truy cập chủ sở hữu trên Lệnh Đặt trước để đổi lại hoặc hoàn tiền. Việc truy cập vào chỉ Đặt trước sẽ không cho phép bạn tiếp tục hoàn tiền hoặc đổi lại. Yêu cầu chủ sở hữu Yêu cầu Đặt trước cung cấp cho bạn quyền truy cập của chủ sở hữu vào Lệnh Đặt trước
- **Exchange sách mới:** Bạn có thể trao đổi đặt trước để giữ lại một loại đặt trước khác – không có **hình thức trừng phạt nào** đối với việc trao đổi đặt trước. Tổng cam kết với việc đặt trước mới phải lớn hơn tổng số tiền hoàn lại cho việc đặt trước đã trao đổi và các khoản thanh toán hàng tháng trong tương lai (nếu có)
- **Chính sách hoàn tiền:** Tổng tiền hoàn trả và các khoản thanh toán trong tương lai đã hủy bỏ không được vượt quá $50.000 USD trong một cửa sổ liên kết 12 tháng. Hiện tại, **chúng tôi không tính bất kỳ khoản tiền hoàn lại nào** cho việc hoàn tiền nhưng có thể tính phí cho các khoản hoàn tiền trong tương lai

**Ngoại lệ:** Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp hàng

- **Api / PS / CLI** không sẵn có để hủy bỏ và hoàn tiền cho trao đổi tự phục vụ và hoàn tiền cho Việc đặt trước [Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp khách hàng. Hỗ trợ các loại đăng ký khác của Chính phủ Hoa Kỳ bao gồm Thanh toán Khi Di chuyển và CSP

Tìm hiểu thêm: [Cách xử lý giao dịch](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) trả lại và trao đổi Tìm hiểu thêm: chính sách [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) hoàn tiền Các câu hỏi khác: Truy nhập tài liệu phiên bản [dành riêng](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange một phiên bản dành riêng hiện có (Tự phục vụ)**

Bạn có thể đổi phần bảo lưu cho một phần bảo lưu khác có cùng loại. Bạn cũng có thể hoàn tiền cho việc đặt trước, tối đa $50.000 USD mỗi năm, nếu bạn không cần nữa. Tính năng trao đổi và hủy bỏ tự phục vụ không sẵn dùng cho khách hàng của Chính phủ Hoa Thỏa thuận Doanh nghiệp khách hàng. Hỗ trợ các loại đăng ký khác của Chính phủ Hoa Kỳ, bao gồm Thanh toán Khi Di chuyển và CSP. Bạn phải có quyền truy cập của chủ sở hữu trên Lệnh Đặt trước để đổi lại hoặc hoàn lại tiền bảo lưu hiện có.

Các bước sau đây sẽ hướng dẫn quy trình hoàn tất giao dịch

1.Đăng nhập vào cổng thông [tin Azure của bạn.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Chọn đặt trước mà bạn muốn hoàn tiền và **bấm Exchange** 2.Chọn sản phẩm VM mà bạn muốn mua và nhập số lượng. Hãy đảm bảo rằng tổng mua hàng mới lớn hơn tổng hoàn vốn Xác định [kích cỡ phù hợp trước khi mua.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Xem lại và hoàn tất giao dịch

**Hoàn tiền cho bản thể hiện đã đặt trước**

Để hoàn tiền cho việc đặt trước, hãy đi tới Chi **tiết Đặt trước và** bấm vào Hoàn **tiền**

**Pro hoàn tiền được xếp hạng cao nhất:**

**Pro dụ về yêu cầu tối thiểu và hoàn tiền cho việc đổi** trả Ví dụ về đặt trước mặt trước:

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

**Không thể thấy hóa đơn cho kỳ thanh toán cuối cùng**

Một số lý do có thể khiến bạn có thể không thấy hóa đơn:

- Bạn có số tiền tín dụng hàng tháng kèm theo đăng ký không vượt quá hoặc bạn có Bản dùng thử Miễn phí. Hóa đơn chỉ được tạo khi bạn nợ tiền
- Thời gian chưa đến 30 ngày kể từ ngày bạn đăng ký Azure
- Hóa đơn chưa được tạo. Chờ đến cuối kỳ thanh toán
- Nếu bạn không phải là Người quản trị Tài khoản, các hóa đơn cũ hơn có thể không có sẵn cho bạn

**Tải xuống hóa đơn của bạn từ cổng thông tin Azure (.pdf)**

- Chọn đăng ký của bạn từ [trang Đăng ký](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) trong cổng thông tin Azure với tư cách là người dùng có quyền truy nhập vào hóa [đơn](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Chọn **Hóa đơn**
- Bấm **vào Tải xuống Hóa** đơn để xem bản sao hóa đơn PDF của bạn. Nếu có thông **báo Không khả dụng**, hãy xem mục Tại sao tôi không thấy hóa đơn cho kỳ thanh toán gần [nhất?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Nhận hóa đơn của bạn qua email (.pdf)**

- Chọn đăng ký của bạn [từ trang Đăng](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ký. Bấm **Hóa đơn rồi** Gửi hóa đơn của tôi qua email
- Bấm chọn **tham gia** và chấp nhận các điều khoản. Bạn sẽ phải chọn tham gia cho từng đăng ký bạn sở hữu

Lưu ý: Nếu bạn không nhận được email sau khi làm theo các bước, hãy đảm bảo rằng địa chỉ email của bạn là chính xác trong tùy chọn thông [tin liên lạc trên hồ sơ của bạn](https://account.windowsazure.com/profile)

**Tải xuống dữ liệu sử dụng của bạn từ cổng thông tin Azure**

- Đăng nhập vào Trung [tâm Tài khoản Azure với](https://account.windowsazure.com/Subscriptions) tư cách là Người quản trị Tài [khoản](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Chọn đăng ký mà bạn muốn có thông tin về hóa đơn và mức sử dụng
- Chọn Lịch **sử Thanh toán**
- Chọn **Xem Bản sao kê Hiện** tại để xem ước tính chi phí của bạn tại thời điểm tạo ước tính
- Chọn **Tải xuống mức sử** dụng để tải xuống dữ liệu sử dụng hàng ngày dưới dạng tệp CSV. Nếu bạn thấy hai phiên bản sẵn dùng, hãy tải xuống phiên bản 2

Câu hỏi khác: [Truy cập tài liệu phiên bản dành riêng](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tài liệu được Đề xuất**

- [Thông tin cơ bản về thanh toán](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Hiểu rõ cách áp dụng chiết khấu cho Phiên bản Bảo lưu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tải xuống hoặc xem hóa đơn thanh toán Azure và dữ liệu sử dụng hàng ngày của bạn](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Hiểu rõ cách áp dụng chiết khấu cho Phiên bản Bảo lưu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Hiểu rõ mức sử dụng Phiên bản Bảo lưu cho đăng ký Thanh toán Khi Bạn Sử dụng](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tìm hiểu về cách sử dụng Mẫu Bảo lưu cho đăng ký Doanh nghiệp của bạn](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows phí phần mềm không bao gồm trong các phiên bản Dành riêng](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các Bản thể hiện Bảo lưu trong chương trình Nhà cung cấp Giải pháp Điện toán Đám mây Trung tâm Đối tác (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)