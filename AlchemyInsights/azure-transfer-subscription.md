---
title: Chuyển quyền sở hữu thanh toán Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922239"
---
# <a name="transfer-azure-billing-ownership"></a>Chuyển quyền sở hữu thanh toán Azure

Đăng nhập vào [cổng thông tin Azure](https://portal.azure.com/) với tư cách là người quản trị của tài khoản thanh toán có đăng ký mà bạn muốn chuyển. Nếu bạn không chắc chắn nếu bạn là người quản trị, hoặc nếu bạn cần xác định ai, hãy xem [xác định người quản trị thanh toán tài khoản](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Tìm kiếm về **quản lý chi phí + thanh toán**.
- Chọn **đăng ký** từ ngăn bên trái. Tùy thuộc vào quyền truy nhập, bạn có thể cần phải chọn một phạm vi thanh toán, sau đó **thuê** bao hoặc **đăng ký Azure**.
- Chọn **chuyển quyền sở hữu thanh toán** cho thuê bao mà bạn muốn chuyển
- Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản đó sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển**
- Người dùng nhận được một email với các hướng dẫn để xem lại yêu cầu chuyển của bạn. Để phê duyệt yêu cầu chuyển, người dùng sẽ chọn liên kết trong email và làm theo hướng dẫn.

**Lưu ý** : nếu bạn chuyển quyền sở hữu thanh toán của gói đăng ký của mình vào tài khoản của người dùng trong một đối tượng thuê Azure AD khác, tất cả các [điều khiển truy nhập dựa trên vai trò (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)để quản lý tài nguyên trong đăng ký đều bị loại bỏ vĩnh viễn. Chỉ có chủ sở hữu mới sẽ có quyền truy nhập để quản lý tài nguyên trong đăng ký. Để biết thêm thông tin, hãy xem mục [chuyển gói đăng ký cho người dùng trong một đối tượng thuê AZURE AD khác](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tài liệu được đề xuất**

- [Chuyển quyền sở hữu thanh toán của một thuê bao Azure sang một tài khoản khác](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Giới thiệu về việc chuyển quyền sở hữu thanh toán cho một thuê bao Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Chuyển giao Visual Studio, mạng Microsoft Partner (MPN) và trả tiền theo mức sử dụng cho các thuê bao dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Chuyển câu hỏi về quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Khắc phục sự cố về quyền sở hữu truyền](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
