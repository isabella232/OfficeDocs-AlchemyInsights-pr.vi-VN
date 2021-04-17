---
title: Thanh toán cho bản dùng phiên bản dự trữ
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820344"
---
# <a name="billing-for-reserved-instance-purchase"></a>Thanh toán cho bản dùng phiên bản dự trữ

Mua phiên bản dự trữ được tính phí cho phương thức thanh toán gắn với đăng ký mà bạn chọn tại thời điểm mua. Loại đăng ký phải là một thỏa thuận doanh nghiệp (cung cấp số: MS-AZR-0017P), Pay-as-you-go (offer Number: MS-AZR-0003P), Microsoft customer thỏa thuận hoặc CPC.

- Đối với thuê bao doanh nghiệp, các khoản phí sẽ được khấu trừ từ số dư cam kết tiền tệ của đăng ký hoặc tính phí là quá hạn
- Đối với gói đăng ký thanh toán-as-you-go, các khoản phí sẽ được lập hóa đơn vào thẻ tín dụng hoặc phương thức thanh toán hóa đơn trên thuê bao

**Hủy đặt trước**

- **Tự phục vụ:** Bạn có thể hủy bỏ hoặc trao đổi một bản thể hiện riêng cho bản thân bạn bằng cách sử dụng [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Chọn đặt trước và bấm vào hoàn tiền hoặc trao đổi. Lưu ý rằng bạn phải có quyền truy cập vào chủ sở hữu thứ tự đặt trước để trao đổi hoặc hoàn tiền. Quyền truy nhập chỉ đặt phòng sẽ không cho phép bạn tiếp tục hoàn tiền hoặc trao đổi. Đặt yêu cầu người sở hữu đặt trước để cấp cho bạn quyền truy nhập vào thứ tự đặt trước
- **Chính sách Exchange:** Bạn có thể trao đổi một đặt trước để đặt một lần nữa cùng loại – không có hình **phạt nào** về Exchange. Tổng các cam kết với việc Đặt phòng mới phải lớn hơn tổng của số tiền hoàn tiền của Đặt phòng và các khoản thanh toán hàng tháng trong tương lai (nếu có)
- **Chính sách hoàn tiền:** Tổng hoàn tiền và các khoản thanh toán trong tương lai không thể vượt quá $50.000 USD trong một cửa sổ lăn 12 tháng. **Hiện tại chúng tôi không tính phí bất kỳ hình phạt nào** khi hoàn tiền nhưng có thể tính phí tiền bồi hoàn trong tương lai

**Ngoại lệ:** Tự phục vụ Exchange và hủy bỏ khả năng không sẵn dùng cho khách hàng thỏa thuận doanh nghiệp của chính phủ Hoa Kỳ

- Hỗ trợ **API/PS/CLI** không sẵn dùng để hủy bỏ và hoàn tiền lại [trao đổi tự phục vụ và hoàn tiền cho Azure RESERVATIONS](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Tự phục vụ Exchange và hủy bỏ khả năng không sẵn dùng cho khách hàng thỏa thuận doanh nghiệp của chính phủ Hoa Kỳ. Các loại đăng ký của chính phủ Hoa Kỳ khác bao gồm thanh toán-như-bạn-Go và CPC được hỗ trợ

Tìm hiểu thêm: [cách xử lý giao dịch và trao đổi sẽ](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) tìm hiểu thêm: [chính sách trao đổi và hoàn tiền](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) các câu hỏi khác: [truy cập vào](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) tài liệu dự phiên bản dự trữ

**Trao đổi phiên bản dự trữ hiện có (tự phục vụ)**

Bạn có thể trao đổi đặt trước để đặt trước một kiểu khác của cùng một loại. Bạn cũng có thể hoàn tiền lại một lúc đặt trước, tối đa $50.000 USD mỗi năm, nếu bạn không còn cần đến. Tự phục vụ Exchange và hủy bỏ khả năng không sẵn dùng cho khách hàng thỏa thuận doanh nghiệp của chính phủ Hoa Kỳ. Các loại đăng ký của chính phủ Hoa Kỳ khác bao gồm thanh toán-như-bạn-Go và CPC được hỗ trợ. Bạn phải có quyền truy nhập của chủ sở hữu để đặt trước để trao đổi hoặc hoàn tiền đặt trước hiện tại.

Các bước sau đây sẽ hướng dẫn quy trình để hoàn tất giao dịch

1. đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)của bạn. Chọn Đặt phòng mà bạn muốn hoàn tiền và bấm **Exchange** 2. chọn sản phẩm VM mà bạn muốn mua và nhập số lượng. Hãy đảm bảo rằng tổng mua mới có nhiều hơn tổng trả về [xác định kích cỡ phù hợp trước khi bạn mua](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. xem lại và hoàn tất giao dịch

**Hoàn tiền cho một ví dụ dành riêng**

Để hoàn tiền lại một lúc đặt trước, hãy đi tới **chi tiết đặt trước** và bấm **hoàn tiền**

**Hoàn tiền được đánh giá Pro:**

Các **ví dụ Pro-suất ăn và yêu cầu tối thiểu để hoàn tiền và trao đổi** Ví dụ về đặt trước khi trả trước:

- Bạn mua một thuật ngữ RI năm cho $120 vào ngày 1 tháng 1
- Vào ngày 07 tháng tư bạn muốn hoàn tiền hoặc trao đổi đặt chỗ này
- Kể từ khi đặt trước đã được trực tiếp cho 97 ngày, bạn sẽ nhận được (1-97/365) * $120 trở lại. (ví dụ như $88,1). Hiện tại không có hình phạt khi hoàn tiền
- Nếu việc trao đổi, mua mới của bạn phải lớn hơn $88,1
- Hiện không có hình phạt nào khi hoàn tiền

**Ví dụ về lập hóa đơn đặt phòng:**

- Bạn mua một thuật ngữ RI năm cho $10 mỗi tháng
- Vào ngày 07 tháng tư bạn muốn hoàn tiền hoặc trao đổi đặt chỗ này
- Kể từ khi thanh toán cuối cùng đã xảy ra 7 ngày, bạn sẽ nhận được (1-7/31) * $10 trở lại. (ví dụ như $7,74)
- Các khoản thanh toán trong tương lai đã bị hủy là $80. Hiện tại không có hình phạt khi hoàn tiền
- Việc hủy bỏ này sẽ trừ $87,74 từ bạn là giới hạn hoàn tiền $50.000
- Nếu trao đổi, giá trị tổng của mua mới sẽ lớn hơn $87,74

**Không thể xem hóa đơn cho thời hạn thanh toán cuối cùng**

Một số lý do có thể có thể bạn không nhìn thấy hóa đơn:

- Bạn có số tiền tín dụng hàng tháng với đăng ký của mình mà bạn chưa vượt quá hoặc bạn có bản dùng thử miễn phí. Hóa đơn chỉ được tạo ra khi bạn nợ tiền
- Nó nhỏ hơn 30 ngày kể từ ngày bạn đã đăng ký Azure
- Hóa đơn không được tạo ra. Chờ cho đến khi kết thúc thời hạn thanh toán
- Nếu bạn không phải là người quản trị tài khoản, các hóa đơn cũ hơn có thể không sẵn dùng cho bạn

**Tải xuống hóa đơn của bạn từ Azure Portal (. PDF)**

- Chọn đăng ký của bạn từ trang [đăng ký](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) trong Azure Portal [với tư cách là người dùng có quyền truy nhập vào hóa đơn](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Chọn hóa **đơn**
- Bấm **tải xuống hóa đơn** để xem bản sao của hóa đơn PDF của bạn. Nếu thông báo **không sẵn dùng**, hãy xem [tại sao tôi không nhìn thấy hóa đơn cho thời hạn thanh toán cuối cùng?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Nhận hóa đơn của bạn trong email (. PDF)**

- Chọn đăng ký của bạn từ trang [đăng ký](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Bấm hóa **đơn** sau đó gửi email hóa đơn của tôi
- Bấm vào **chọn tham** gia và chấp nhận các điều khoản. Bạn sẽ phải chọn tham gia cho mỗi đăng ký của riêng bạn

Lưu ý: nếu bạn không nhận được email sau khi thực hiện theo các bước này, hãy đảm bảo địa chỉ email của bạn là chính xác trong [tùy chọn giao tiếp trên hồ sơ của bạn](https://account.windowsazure.com/profile)

**Tải xuống dữ liệu sử dụng của bạn từ cổng thông tin Azure**

- Đăng nhập vào [Trung tâm tài khoản Azure](https://account.windowsazure.com/Subscriptions) làm người [quản trị tài khoản](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Chọn đăng ký mà bạn muốn hóa đơn và thông tin về sử dụng
- Chọn **lịch sử thanh toán**
- Chọn **xem báo cáo hiện tại** để xem ước tính phí của bạn tại thời điểm ước tính được tạo ra
- Chọn **tải xuống việc sử dụng** để tải xuống dữ liệu sử dụng hàng ngày dưới dạng tệp CSV. Nếu bạn thấy hai phiên bản sẵn dùng, tải xuống phiên bản 2

Các câu hỏi khác: [truy cập](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) tài liệu dự phiên bản dự trữ

**Tài liệu được đề xuất**

- [Cơ bản về thanh toán](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tìm hiểu cách áp dụng chiết khấu Phiên bản dành riêng](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tải xuống hoặc xem hóa đơn Azure thanh toán của bạn và dữ liệu sử dụng hàng ngày](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tìm hiểu cách áp dụng chiết khấu Phiên bản dành riêng](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tìm hiểu về việc sử dụng bản thể hiện dành riêng cho thuê bao trả tiền của bạn](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tìm hiểu về việc sử dụng bản thể hiện dành cho doanh nghiệp của bạn](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các chi phí phần mềm Windows không được bao gồm trong các phiên bản dự trữ](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các phiên bản dành riêng trong chương trình nhà cung cấp giải pháp điện toán đám mây đối tác (CPC)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)