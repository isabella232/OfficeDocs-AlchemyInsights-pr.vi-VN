---
title: Các loại đăng ký được hỗ trợ
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808177"
---
# <a name="supported-subscription-types"></a>Các loại đăng ký được hỗ trợ

Vui lòng xem lại các loại đăng ký được hỗ trợ để tiếp tục tiếp tục.

[Các loại đăng ký được hỗ trợ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Chuyển quyền sở hữu thanh toán**

Azure Portal là người [quản trị tài khoản](https://ms.portal.azure.com/) của tài khoản thanh toán có thuê bao mà bạn muốn chuyển

- Tìm kiếm về **quản lý chi phí + thanh toán** . Chọn **thuê** bao từ ngăn bên trái. Tùy thuộc vào quyền truy nhập, bạn có thể cần phải chọn một phạm vi thanh toán, sau đó **thuê** bao hoặc **đăng ký Azure** .
- Chọn chuyển quyền sở hữu thanh toán cho thuê bao mà bạn muốn chuyển
- Nhập địa chỉ email của người dùng là người quản trị thanh toán của tài khoản đó sẽ là chủ sở hữu mới cho đăng ký, rồi chọn **gửi yêu cầu chuyển**
- Người dùng nhận được một email với các hướng dẫn để xem lại yêu cầu chuyển của bạn. Để phê duyệt yêu cầu chuyển, người dùng sẽ chọn liên kết trong email và làm theo hướng dẫn.

Lưu ý: nếu bạn chuyển quyền sở hữu thanh toán của gói đăng ký của mình vào tài khoản của người dùng trong một đối tượng thuê Azure AD khác, tất cả các [điều khiển truy nhập dựa trên vai trò (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) để quản lý tài nguyên trong đăng ký đều bị loại bỏ vĩnh viễn. Chỉ có chủ sở hữu mới sẽ có quyền truy nhập để quản lý tài nguyên trong đăng ký. Để biết thêm thông tin, hãy xem mục [chuyển gói đăng ký cho người dùng trong một đối tượng thuê AZURE AD khác](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Chuyển quyền sở hữu đăng ký**

Quyền sở hữu đăng ký chuyển giao truy nhập dựa trên vai trò điều kiện tiên quyết (RBAC) để quản lý tài nguyên trong đăng ký bị mất quyền truy nhập của họ. Để biết thêm thông tin về việc thêm một thuê bao hiện có cho một đối tượng thuê, hãy xem [liên kết hoặc thêm đăng ký Azure vào Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Chuyển gói đăng ký với một số lượng tồn đọng hiện có từ chu kỳ thanh toán hiện tại sẽ không được chuyển sang các công cụ thanh toán mới trong tài khoản mới. Thông tin chỉ khả dụng cho người dùng trong tài khoản mới là chi phí cuối của tháng cho thuê bao của bạn. Phần còn lại của lịch sử sử dụng và thanh toán sẽ không chuyển giao với đăng ký.
- Chuyển quyền sở hữu thanh toán của gói đăng ký thỏa thuận doanh nghiệp (EA) hiện đang được hỗ trợ trong cổng thông tin thỏa thuận doanh nghiệp
- Chuyển một thuê bao theo định hướng tín dụng như Visual Studio, BizSpark, mạng Microsoft Partner cho một người dùng mới yêu cầu phải có giấy phép trực quan của một máy tính đối tác mạng/Microsoft để chấp nhận yêu cầu chuyển
- Tất cả các tài nguyên như máy ảo, ổ đĩa và trang web được chuyển đến tài khoản mới thành công. Các tài nguyên sau đây có thể bị ảnh hưởng trong chuyển giao thuê bao chéo:

**Dịch vụ tên miền Azure AD**

Khung vòm phím Azure

- [Người dùng và cơ sở dữ liệu liên quan SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) có thể bị ảnh hưởng, đặc biệt là nếu khách hàng sử dụng xác thực liên quan đến Azure Active Directory
- Các **dịch vụ ứng dụng** được cấu hình với chứng thực Azure Active Directory có thể bị ảnh hưởng
- **Nhóm Visual Studio** Tài khoản Dịch vụ kết nối với đăng ký Azure có thể tạm thời mất quyền truy nhập khi đăng ký Azure đã kết nối bị hủy bỏ

**Tài liệu được đề xuất**

Các bước sau khi chấp nhận quyền sở hữu thanh toán:

- Để duy trì quyền sở hữu thanh toán, nhưng thay đổi loại đăng ký của bạn, hãy tham khảo: [chuyển đổi đăng ký Azure của bạn sang một lời mời khác](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Chuyển giao Visual Studio, mạng Microsoft Partner (MPN) và trả tiền theo mức sử dụng cho các thuê bao dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Chuyển quyền sở hữu thanh toán của các gói đăng ký thỏa thuận doanh nghiệp (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Chuyển câu hỏi về quyền sở hữu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Khắc phục sự cố về quyền sở hữu truyền](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)