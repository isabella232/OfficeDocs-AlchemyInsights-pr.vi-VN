---
title: Cho phép quản lý chi phí
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678777"
---
# <a name="enable-cost-management"></a>Cho phép quản lý chi phí

**' Chi phí nào bị vô hiệu cho tổ chức của bạn có nghĩa là gì?**

Các tổ chức sử dụng thỏa thuận doanh nghiệp (EA) hoặc các tài khoản thỏa thuận Microsoft customer (MCA) có thể tắt quyền truy nhập vào thông tin chi phí và thông tin về giá.

Sau khi đăng nhập vào Azure Portal, họ có thể sử dụng các API thanh toán để lập trình các hóa đơn (sau khi chọn tham gia) và chi tiết về mức sử dụng.

**Cách để cho phép người dùng bổ sung truy nhập hóa đơn**

1. Đi đến **lưỡi đăng ký** trong Azure Portal.
2. Chọn hóa **đơn** và sau đó **truy nhập vào hóa đơn**.
3. Bật truy nhập, tiếp theo là lưu các thay đổi, để cho phép người dùng trong vai trò đăng ký-phạm vi để tải xuống hóa đơn.

> [!NOTE]
> Người quản trị tài khoản cũng có thể cấu hình để có các hóa đơn được gửi qua email. Để tìm hiểu thêm, hãy xem [mục nhận hóa đơn của bạn trong email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Cách thêm người dùng vào vai trò bộ đọc thanh toán**

1. Đi đến **lưỡi đăng ký** trong Azure Portal.
2. Chọn **Access Control (iam)** , rồi bấm **Thêm**.
3. Chọn bộ **đọc thanh toán** trong trang **chọn vai trò** .
4. Nhập email của người dùng mà bạn muốn mời, rồi bấm **OK** để gửi lời mời.
5. Làm theo hướng dẫn được cung cấp trong email mời để đăng nhập với tư cách là bộ đọc thanh toán. Để biết thêm thông tin, hãy xem [cấp quyền truy nhập vào thanh toán](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Tài liệu được đề xuất**

- [Kích hoạt các dạng xem DA và AO qua EA Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Chi phí bao gồm trong quản lý chi phí](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Cung cấp Microsoft Azure được hỗ trợ](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Xem lại chi phí trong phân tích chi phí](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Cung cấp quyền truy nhập vào thông tin thanh toán](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kiểm tra quyền truy nhập vào thỏa thuận khách hàng của Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






