---
title: Các loại đăng ký được hỗ trợ
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
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072182"
---
# <a name="supported-subscription-types"></a>Các loại đăng ký được hỗ trợ

Vui lòng xem lại các loại đăng ký được hỗ trợ để tiếp tục thêm.

[Các loại đăng ký được hỗ trợ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Chuyển quyền sở hữu thanh toán**

Cổng thông tin Azure với [tư cách là Người](https://ms.portal.azure.com/) quản trị Tài khoản của tài khoản thanh toán có đăng ký mà bạn muốn chuyển

- Tìm kiếm về **Quản lý Chi phí + Hóa đơn.** Chọn **Đăng ký** từ ngăn bên trái. Tùy thuộc vào quyền truy nhập, bạn có thể cần chọn một phạm vi thanh **toán, rồi chọn Đăng ký** hoặc Đăng ký **Azure.**
- Chọn Chuyển quyền sở hữu thanh toán cho đăng ký mà bạn muốn chuyển
- Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển khoản**
- Người dùng nhận được email kèm theo hướng dẫn để xem lại yêu cầu chuyển giao của bạn. Để chấp thuận yêu cầu chuyển, người dùng chọn liên kết trong email và làm theo hướng dẫn.

Lưu ý: Nếu bạn chuyển quyền sở hữu thanh toán cho đăng ký của mình sang tài khoản người dùng trong một đối tượng thuê Azure AD khác, tất cả hoạt động gán kiểm soát truy nhập dựa trên vai trò [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) để quản lý tài nguyên trong đăng ký sẽ bị loại bỏ vĩnh viễn. Chỉ chủ sở hữu mới có quyền truy nhập để quản lý tài nguyên trong đăng ký. Để biết thêm thông tin, xem [mục Chuyển đăng ký cho người dùng trong đối tượng thuê Azure AD khác.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chuyển quyền sở hữu đăng ký**

Vai trò tiên quyết trong Chuyển Quyền sở hữu Đăng ký dựa trên quyền truy nhập (RBAC) để quản lý các tài nguyên trong đăng ký sẽ mất quyền truy nhập. Để biết thêm thông tin về việc thêm đăng ký hiện có cho đối tượng thuê, hãy xem liên kết [hoặc thêm đăng ký Azure vào Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

- Chuyển đăng ký với một số tiền còn nợ hiện tại từ chu kỳ thanh toán hiện tại sẽ không được chuyển sang phương tiện thanh toán mới trong tài khoản mới. Thông tin duy nhất có sẵn cho người dùng trong tài khoản mới là chi phí của tháng trước cho đăng ký của bạn. Phần còn lại của lịch sử sử dụng và thanh toán không chuyển đi cùng với đăng ký.
- Hiện chỉ hỗ trợ chuyển quyền sở Thỏa thuận Doanh nghiệp quyền sở hữu thanh toán của đăng ký (EA) Thỏa thuận Doanh nghiệp Portal
- Việc chuyển đăng ký theo định hướng tín dụng như Visual Studio, BizSpark, Mạng Đối tác của Microsoft cho người dùng mới yêu cầu phải có giấy phép mạng Visual Studio/Đối tác Microsoft để chấp nhận yêu cầu chuyển giao
- Tất cả các tài nguyên như Máy Ảo, đĩa và website chuyển thành công sang tài khoản mới. Các tài nguyên sau đây có thể bị ảnh hưởng trong quá trình chuyển đăng ký nhiều đối tượng thuê:

**Dịch vụ Miền Azure AD**

Tín liệu Khóa Azure

- [SQL người dùng và cơ sở dữ liệu có liên](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) quan có thể bị ảnh hưởng, đặc biệt là khi khách hàng sử dụng xác Azure Active Directory có liên quan
- **Dịch vụ Ứng dụng** được đặt cấu hình Azure Active Directory thể bị ảnh hưởng
- **Visual Studio Team** Các tài khoản dịch vụ được kết nối với gói đăng ký Azure có thể tạm thời mất quyền truy nhập khi đăng ký Azure được kết nối bị hủy bỏ

**Tài liệu được Đề xuất**

Các bước sau khi chấp nhận quyền sở hữu thanh toán:

- Để duy trì quyền sở hữu thanh toán nhưng thay đổi loại đăng ký của bạn, hãy tham khảo: [Chuyển đăng ký Azure của bạn sang một gói đăng ký khác](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Chuyển Visual Studio, Mạng Đối tác của Microsoft (MPN) và Thanh toán khi bạn đi tới đăng ký Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Chuyển quyền sở hữu thanh Thỏa thuận Doanh nghiệp ký (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Câu hỏi thường gặp về chuyển quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Khắc phục sự cố Chuyển quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)