---
title: Tại sao nút thêm ngân sách bị vô hiệu hóa cho tôi?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822657"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Tại sao nút thêm ngân sách bị vô hiệu hóa cho tôi?

Để tạo ngân sách, bạn cần một trong các quyền sau đây:

- Nhóm quản lý, đăng ký, phạm vi nhóm tài nguyên
- Người đóng góp quản lý chi phí
- Tư
- Người đóng góp
- Chỉ dành cho khách hàng doanh nghiệp: đăng ký, Phòng ban, phạm vi tài khoản
- Người quản trị đăng ký (đặt ngân sách tại phạm vi đăng ký)
- Người quản trị bộ phận (đặt ngân sách tại phạm vi phòng ban)
- Chủ sở hữu tài khoản (đặt ngân sách tại phạm vi tài khoản)
- Thỏa thuận khách hàng hiện đại, chỉ: tài khoản thanh toán, Hồ sơ thanh toán, phạm vi của phần hóa đơn
- Người tạo đăng ký Azure

**Tôi đã tạo ngân sách khi chi phí của mình cho tháng hiện tại đã vượt quá ngân sách. Tại sao tôi không nhận được cảnh báo?**  
Nếu bạn đã vượt quá ngưỡng chi phí được đặt trước khi tạo ngân sách cảnh báo sẽ không cháy. Sau khi một vòng tròn mới bắt đầu, nếu bạn vi phạm ngưỡng sau đó cảnh báo sẽ cháy.

**Khi nào tôi nên nhận được cảnh báo sau khi vượt quá một trong những ngưỡng cảnh báo ngân sách được xác định của tôi?**  
Ngân sách được đánh giá mỗi 4 giờ. Phải mất ít nhất 8 giờ cho việc sử dụng dữ liệu để đến hệ thống ngân sách. Cho điều này, các cảnh báo có thể kéo dài 12 giờ để bắn sau khi bạn vượt quá ngưỡng.

**Tại sao nút ngày bắt đầu bị vô hiệu hóa khi tôi chọn một khoảng thời gian đặt lại tháng hoặc thanh toán tháng?**  
Ngân sách được căn chỉnh vào tháng hiện tại hoặc thời hạn thanh toán hiện tại (trong trường hợp được chọn trong tháng thanh toán). Vì vậy, chúng tôi trước khi cư trú giá trị này cho bạn.

**Tại sao tôi không nhìn thấy một đồ thị chi phí của mình trong trải nghiệm tạo ngân sách?**  
Chúng tôi cần tối thiểu 2 tháng dữ liệu chi phí trước khi chúng tôi có thể tạo một đồ thị để hỗ trợ bạn với việc tạo ngân sách.

**Tại sao tôi không thể thiết lập ngân sách đối với một đăng ký tôi vừa tạo?**  
Sau khi tạo đăng ký, dữ liệu sẽ mất 24-48 giờ để xử lý trước khi thiết lập ngân sách chống lại nó.

**Tài nguyên API ngân sách**

- [Ngân sách API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): cung cấp các hoạt động để tạo và Cập Nhật ngân sách. Sử dụng API ngân sách, bạn có thể thiết lập một ngưỡng ngân sách và cấu hình nhiều cảnh báo để bắn khi bạn tiếp cận ngưỡng đó. Cảnh báo có thể kích hoạt email hoặc nhóm hành động Azure để thực hiện tự động hóa. Lưu ý: lọc cho API này không căn chỉnh với truy vấn bộ lọc/kích thước API.
- [API ngân sách v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): tạo ngân sách với các khả năng lọc chi phí lớn hơn v1. Lọc các căn chỉnh cho hợp đồng được sử dụng trong các API truy vấn và kích thước của chúng tôi. Đây là API ngân sách được đề xuất để sử dụng di chuyển về phía trước.
- [Kích thước](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): cung cấp các hoạt động để nhận các kích thước được hỗ trợ cho việc sử dụng của bạn dưới nhiều phạm vi. Sử dụng API kích thước, bạn có thể truy xuất danh sách các kích thước có thể được dùng làm đầu vào để tạo truy vấn bằng API truy vấn.
- [Truy vấn](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): cung cấp các phép toán để có được tổng hợp chi phí và mức sử dụng dữ liệu dựa trên truy vấn mà bạn cung cấp. Sử dụng API truy vấn, bạn có thể xác định việc lọc, sắp xếp và phân nhóm mong muốn của bạn trên tất cả các kích thước sẵn có (được truy nhập từ API kích thước).

**Chi phí dự báo**

**Tại sao tôi không thấy các dự báo về chi phí của mình trong phân tích chi phí?**  
Có nhiều lý do tại sao phép chiếu dự báo có thể bị thiếu cho bạn trong phân tích chi phí, một số người trong số đó là như sau:

1. Nếu dữ liệu chi phí của bạn nhỏ hơn 10 ngày, biểu đồ dự báo sẽ không tải được. Mô hình này đòi hỏi ít nhất 10 ngày so với dữ liệu chi phí gần đây về bản chiếu chính xác
2. Nếu bạn đã chọn ngày lịch sử, thì biểu đồ dự báo sẽ không được hiển thị. Vui lòng chọn một phạm vi ngày với ngày trong tương lai cho biểu đồ dự báo sẽ được hiển thị
3. Nếu tài khoản của bạn có nhiều tiền tệ, biểu đồ dự báo sẽ chỉ có chi phí dự án cho ' tất cả các chi phí trong USD '

**Tại sao dự báo không thay đổi khi tôi thực hiện thay đổi đối với tài nguyên của mình?**  
Mô hình dự báo yêu cầu một vài ngày đến tài khoản cho các thay đổi trong tài khoản và không thực hiện các bản chiếu ngay lập tức dựa trên thay đổi trong tài nguyên  
Để biết các bước lớn hơn của việc tăng hoặc giảm trong tài nguyên, mô hình sẽ mất hơi dài hơn để điều chỉnh những thay đổi này cho tài khoản cho các điểm bất thường

**Tại sao dự báo của tôi tăng sau khi tôi đặt gói mua hoặc mua một thị trường?**  
Mô hình dự báo sẽ xem xét ' chi phí thực tế ' và không tài khoản cho việc sử dụng và mua riêng biệt. Đối với gói mua một lần, mô hình sẽ giảm các bản chiếu sau 10 ngày đến tài khoản để tăng chi phí đột ngột

**Tôi muốn xem các dự báo cho một kích thước đơn (ví dụ. E**  
Dự báo hiện đang hỗ trợ tổng chi phí và không dành cho các mét riêng lẻ. Do đó, khi ' được nhóm theo ' một kích thước, các dự báo sẽ được dành cho tổng tất cả các mục trong kích thước

**Tài liệu được đề xuất**

- [Quản lý chi phí Azure là gì?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các biện pháp tốt nhất về quản lý chi phí Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Phân tích chi phí và chi tiêu của bạn](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Khám phá và phân tích chi phí với phân tích chi phí](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Quản lý chi phí Azure: giá](https://azure.microsoft.com/services/cost-management/#pricing)
- [Xem lại chi phí trong phân tích chi phí](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Hướng dẫn video: tạo ngân sách trong cổng thông tin Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Điều kiện tiên quyết để xem và tùy chỉnh ngân sách](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Tạo và quản lý ngân sách](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Cấu hình tự động hóa với các nhóm hành động Azure và API ngân sách](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Sử dụng các cảnh báo chi phí để theo dõi việc sử dụng và chi tiêu](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Thực hành quản lý chi phí tốt nhất](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video hướng dẫn**

- [Tạo ngân sách trong cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Quản lý chi phí với API ngân sách và nhóm hành động](https://go.microsoft.com/fwlink/?linkid=2147038)