---
title: Chuyển quyền sở hữu thanh toán Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036118"
---
# <a name="transfer-azure-billing-ownership"></a>Chuyển quyền sở hữu thanh toán Azure

Đăng nhập vào cổng [thông tin Azure với](https://portal.azure.com/) tư cách là người quản trị của tài khoản thanh toán có đăng ký mà bạn muốn chuyển. Nếu bạn không chắc mình có phải là người quản trị hay không, hoặc nếu bạn cần xác định ai là người đó, hãy xem mục Xác [định người quản trị thanh toán tài khoản](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Tìm kiếm Quản _lý Chi phí + Hóa đơn._
1. Chọn **Đăng ký** từ ngăn bên trái. Tùy thuộc vào quyền truy nhập, bạn có thể cần chọn một phạm vi thanh **toán, rồi chọn Đăng ký** hoặc Đăng ký **Azure.**
1. Chọn **Chuyển quyền sở hữu thanh** toán cho đăng ký mà bạn muốn chuyển.
1. Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển khoản**.
1. Người dùng nhận được email kèm theo hướng dẫn để xem lại yêu cầu chuyển giao của bạn. Để chấp thuận yêu cầu chuyển, người dùng chọn liên kết trong email và làm theo hướng dẫn.

Xin lưu ý rằng nếu bạn chuyển quyền sở hữu thanh toán của đăng ký sang tài khoản người dùng trong một đối tượng thuê Azure AD khác, tất cả các hoạt động gán kiểm soát truy nhập dựa trên vai trò [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) để quản lý tài nguyên trong đăng ký sẽ bị loại bỏ vĩnh viễn. Chỉ chủ sở hữu mới có quyền truy nhập để quản lý tài nguyên trong đăng ký. Để biết thêm thông tin về cách thay đổi thư mục cho đăng ký, xem mục Chuyển đăng ký [cho người dùng trong đối tượng thuê Azure AD khác.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

_**Ảnh hưởng quan trọng đến hóa đơn**_ của bạn: nếu bạn đã chuyển quyền sở hữu thanh toán cho một đăng ký Azure, chi phí của bạn sẽ được xếp hạng theo tỷ lệ. Bạn sẽ có thể truy nhập các hóa đơn dưới dạng như sau:  

1. Chọn đăng ký của bạn [từ trang Đăng ký](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)trong cổng thông tin Azure với tư cách là người dùng có quyền truy nhập vào hóa    [đơn,](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)sau đó chọn **Hóa đơn**.
1. Bấm **vào Tải xuống Hóa** đơn để xem bản sao hóa đơn PDF của   bạn. Nếu tùy chọn này _có thông báo Không_ khả dụng , hãy xem tại sao tôi không thấy hóa đơn cho kỳ thanh toán gần [nhất?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Bạn cũng có thể xem  mức sử dụng hàng ngày bằng cách bấm vào thời gian thanh toán để nhận bản PDF cho hóa đơn của bạn và bản sao tệp sử dụng hàng ngày chi tiết (.CSV). Để biết thêm thông tin, hãy xem [Lấy hóa đơn và dữ liệu sử dụng](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tài liệu được Đề xuất**

- [Chuyển quyền sở hữu thanh toán của đăng ký Azure sang một tài khoản khác](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Thông tin về việc chuyển quyền sở hữu thanh toán cho đăng ký Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Chuyển Visual Studio, Mạng Đối tác của Microsoft (MPN) và Thanh toán khi bạn đi tới đăng ký Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Câu hỏi thường gặp về chuyển quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Khắc phục sự cố Chuyển quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
