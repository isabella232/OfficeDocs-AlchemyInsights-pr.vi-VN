---
title: Tại sao nút Thêm ngân sách lại bị vô hiệu hóa cho tôi?
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
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954713"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Tại sao nút Thêm ngân sách lại bị vô hiệu hóa cho tôi?

Để tạo ngân sách, bạn cần một trong các quyền sau đây:

- Phạm vi Nhóm Quản lý, Đăng ký, Nhóm Tài nguyên
- Người đóng góp Quản lý Chi phí
- Chủ sở hữu
- Người đóng góp
- Chỉ Dành cho Khách hàng Doanh nghiệp: Đăng ký, Bộ phận, Phạm vi Tài khoản
- Người quản trị Đăng ký (đặt ngân sách ở phạm vi Đăng ký)
- Người quản trị Bộ phận (đặt ngân sách ở phạm vi Bộ phận)
- Chủ sở hữu Tài khoản (đặt ngân sách ở phạm vi Tài khoản)
- Chỉ Thỏa thuận Khách hàng Hiện đại: Tài khoản Thanh toán, Hồ sơ Thanh toán, Phạm vi Phần Hóa đơn
- Người tạo đăng ký Azure

**Tôi đã tạo ngân sách khi chi phí cho tháng hiện tại đã vượt quá ngân sách. Tại sao tôi không nhận được cảnh báo?**  
Nếu bạn đã vượt quá ngưỡng chi phí cho trước khi tạo ngân sách mà cảnh báo đó sẽ không kích hoạt. Sau khi chu kỳ mới bắt đầu, nếu bạn vi phạm ngưỡng thì cảnh báo sẽ khởi động.

**Khi nào tôi nên nhận cảnh báo sau khi vượt quá một trong những ngưỡng cảnh báo ngân sách đã xác định của mình?**  
Ngân sách được đánh giá 4 giờ một lần. Mất ít nhất 8 giờ để dữ liệu sử dụng đạt đến hệ thống ngân sách. Với điều này, các cảnh báo có thể mất tới 12 giờ để kích hoạt sau khi bạn vượt quá ngưỡng.

**Tại sao nút Ngày bắt đầu bị tắt khi tôi chọn thời gian đặt lại Tháng hoặc Tháng thanh toán?**  
Ngân sách được căn chỉnh theo tháng trên lịch hoặc thời gian thanh toán hiện tại (trong trường hợp Đã chọn Tháng Thanh toán). Do đó, chúng tôi sẽ đưa vào trước giá trị này cho bạn.

**Tại sao tôi không nhìn thấy một đồ thị chi phí của tôi trong trải nghiệm tạo ngân sách?**  
Chúng tôi cần dữ liệu chi phí tối thiểu 2 tháng trước khi có thể hiển thị đồ thị nhằm hỗ trợ bạn tạo ngân sách.

**Tại sao tôi không thể đặt ngân sách cho đăng ký tôi vừa tạo?**  
Sau khi tạo đăng ký, dữ liệu cần 24-48 giờ để xử lý trước khi đặt ngân sách cho đăng ký đó.

**Tài nguyên API Ngân sách**

- [API Ngân sách v1: Cung](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)cấp các thao tác để tạo và cập nhật ngân sách. Sử dụng API Ngân sách, bạn có thể đặt ngưỡng ngân sách và đặt cấu hình cho nhiều cảnh báo để phát hoạt khi bạn đạt đến ngưỡng đó. Cảnh báo có thể kích hoạt email hoặc Nhóm Hành động Azure để thực hiện tự động hóa. Lưu ý: Việc lọc đối với API này không phù hợp với kích thước / lọc API truy vấn.
- [API Ngân sách v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Tạo ngân sách với khả năng lọc chi phí lớn hơn v1. Tính năng lọc phù hợp với hợp đồng được sử dụng trong API Truy vấn và Kích thước của chúng tôi. Đây là API ngân sách được đề xuất để sử dụng trong tương lai.
- [Kích thước](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Cung cấp các thao tác để có được các kích thước được hỗ trợ cho việc sử dụng của bạn trong một loạt các phạm vi. Sử dụng API Chiều, bạn có thể truy xuất danh sách kích thước có thể được sử dụng làm đầu vào để tạo truy vấn với API Truy vấn.
- [Truy vấn:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Cung cấp các thao tác để có được chi phí tổng hợp và dữ liệu sử dụng dựa trên truy vấn bạn cung cấp. Sử dụng API truy vấn, bạn có thể chỉ định lọc, sắp xếp và nhóm mong muốn của mình trên tất cả các kích thước sẵn có (được truy nhập từ API Chiều).

**Chi phí dự báo**

**Tại sao tôi không thấy các dự báo cho chi phí của mình trong Phân tích Chi phí?**  
Có nhiều lý do tại sao chức năng chiếu dự báo có thể bị thiếu trong Phân tích Chi phí, một số nguyên nhân trong số đó là:

1. Nếu dữ liệu chi phí của bạn cách đây dưới 10 ngày, biểu đồ dự báo sẽ không tải. Mô hình này yêu cầu ít nhất 10 ngày dữ liệu chi phí gần đây để chiếu chính xác
2. Nếu bạn đã chọn ngày trong lịch sử, biểu đồ dự báo sẽ không hiển thị. Vui lòng chọn phạm vi ngày với ngày trong tương lai để biểu đồ dự báo được hiển thị
3. Nếu tài khoản của bạn có nhiều loại tiền tệ, biểu đồ dự báo sẽ chỉ chi phí dự án cho 'Tất cả chi phí tính bằng USD'

**Tại sao dự báo không thay đổi khi tôi thực hiện thay đổi đối với tài nguyên của mình?**  
Mô hình dự báo cần một vài ngày để tính đến các thay đổi trong tài khoản và không thực hiện dự đoán ngay lập tức dựa trên sự thay đổi trong tài nguyên  
Đối với các bước tăng hay giảm tài nguyên lớn hơn, mô hình sẽ mất nhiều thời gian hơn để điều chỉnh những thay đổi này, để giải quyết các bất thường

**Tại sao dự báo của tôi tăng sau khi tôi đặt trước hoặc mua Marketplace?**  
Mô hình dự báo xem 'Chi phí Thực tế' của bạn và không tính đến việc sử dụng và mua riêng. Đối với mua hàng một lần, mô hình sẽ giảm lượng chiếu sau 10 ngày để giải quyết sự tăng đột ngột chi phí

**Tôi muốn xem các dự báo cho một chiều (ví dụ: Đồng hồ đo)**  
Dự báo hiện hỗ trợ chiếu tổng chi phí chứ không phải cho mét riêng lẻ. Vì thế, khi 'Nhóm theo' một chiều, các dự đoán sẽ cho tổng cộng của tất cả các mục trong chiều

**Tài liệu được Đề xuất**

- [Quản lý Chi phí Azure là gì?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các phương pháp tốt nhất về Quản lý Chi phí Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Phân tích chi phí và chi tiêu của bạn](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Khám phá và phân tích chi phí với phân tích Chi phí](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Quản lý Chi phí Azure: Giá](https://azure.microsoft.com/services/cost-management/#pricing)
- [Xem lại chi phí trong phân tích chi phí](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video hướng dẫn: Tạo ngân sách trong cổng thông tin Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Điều kiện tiên quyết để xem và tùy chỉnh ngân sách](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Tạo và quản lý ngân sách](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Đặt cấu hình tự động hóa với API Nhóm Hành động và Ngân sách Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Sử dụng cảnh báo chi phí để giám sát việc sử dụng và chi tiêu](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Các cách thực hành tốt nhất về Quản lý Chi phí](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video hướng dẫn**

- [Tạo ngân sách trong cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Quản lý chi phí với API Ngân sách và Nhóm Hành động](https://go.microsoft.com/fwlink/?linkid=2147038)