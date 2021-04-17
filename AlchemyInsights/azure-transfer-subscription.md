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
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820632"
---
# <a name="transfer-azure-billing-ownership"></a>Chuyển quyền sở hữu thanh toán Azure

Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/) với tư cách là người quản trị của tài khoản thanh toán có đăng ký mà bạn muốn chuyển. Nếu bạn không chắc chắn nếu bạn là người quản trị, hoặc nếu bạn cần xác định ai, hãy xem [xác định người quản trị thanh toán tài khoản](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Tìm kiếm _quản lý chi phí + thanh toán_.
1. Chọn **đăng ký** từ ngăn bên trái. Tùy thuộc vào quyền truy nhập, bạn có thể cần phải chọn một phạm vi thanh toán, sau đó **thuê** bao hoặc **đăng ký Azure**.
1. Chọn **chuyển quyền sở hữu thanh toán** cho đăng ký mà bạn muốn chuyển.
1. Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản đó sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển**.
1. Người dùng nhận được một email với các hướng dẫn để xem lại yêu cầu chuyển của bạn. Để phê duyệt yêu cầu chuyển, người dùng sẽ chọn liên kết trong email và làm theo hướng dẫn.

Vui lòng lưu ý rằng nếu bạn chuyển quyền sở hữu thanh toán cho đăng ký của mình vào tài khoản của người dùng trong một đối tượng thuê Azure AD khác, tất cả các [điều khiển truy nhập dựa trên vai trò (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) để quản lý tài nguyên trong đăng ký sẽ bị loại bỏ vĩnh viễn. Chỉ có chủ sở hữu mới sẽ có quyền truy nhập để quản lý tài nguyên trong đăng ký. Để biết thêm thông tin về cách thay đổi thư mục cho một thuê bao, hãy xem [chuyển gói đăng ký cho người dùng trong một đối tượng thuê khác AZURE AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Tác động quan trọng đối với hóa đơn của bạn**_: nếu bạn đã chuyển quyền sở hữu thanh toán cho một thuê bao Azure, các chi phí của bạn sẽ được xếp hạng Pro. Bạn sẽ có thể truy nhập các hóa đơn theo những điều sau đây:  

1. Chọn đăng ký của bạn từ [trang đăng ký](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)   trong cổng thông tin Azure với tư [cách là người dùng có quyền truy nhập vào hóa đơn](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), sau đó chọn hóa **đơn**.
1. Bấm **tải xuống hóa đơn**   để xem bản sao của hóa đơn PDF của bạn. Nếu thông báo _không sẵn dùng_, hãy xem [tại sao tôi không nhìn thấy hóa đơn cho thời hạn thanh toán cuối cùng?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Bạn cũng có thể xem sử dụng hàng ngày của mình bằng cách bấm vào **khoảng thời gian thanh toán** để có được PDF hóa đơn của bạn và bản sao của tệp sử dụng hàng ngày chi tiết (. CSV). Để biết thêm thông tin, hãy xem [lấy hóa đơn và dữ liệu sử dụng](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tài liệu được đề xuất**

- [Chuyển quyền sở hữu thanh toán của một thuê bao Azure sang một tài khoản khác](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Giới thiệu về việc chuyển quyền sở hữu thanh toán cho một thuê bao Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Chuyển giao Visual Studio, mạng Microsoft Partner (MPN) và trả tiền theo mức sử dụng cho các thuê bao dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Chuyển câu hỏi về quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Khắc phục sự cố về quyền sở hữu truyền](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
