---
title: Dịch vụ chuyển-di chuyển tất cả các dịch vụ RDFE sang một đăng ký khác
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692426"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Dịch vụ chuyển-di chuyển tất cả các dịch vụ RDFE sang một đăng ký khác

**Di chuyển tài nguyên**

Tài nguyên Azure có thể được di chuyển đến một thuê bao Azure hoặc nhóm tài nguyên khác dưới cùng một thuê bao bằng Azure Portal, Azure PowerShell, Azure CLI, hoặc API REST để di chuyển tài nguyên.

Trước khi bạn có thể di chuyển tài nguyên, hãy xem:

- [Danh sách kiểm tra trước khi di chuyển tài nguyên](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Các dịch vụ có thể được di chuyển](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cách thức xác thực việc di chuyển](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Di chuyển hướng dẫn cho các dịch vụ](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Để di chuyển các tài nguyên hiện có sang một nhóm tài nguyên khác hoặc đăng ký, bạn có thể sử dụng:

- [Cổng thông tin Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Hướng dẫn: [di chuyển các tài nguyên Azure đến một nhóm tài nguyên hoặc đăng ký khác](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Khắc phục sự cố lỗi với Azure Resource Manager**

Tham khảo các bài viết dưới đây để tìm hiểu về một số lỗi triển khai Azure thông thường và nhận thông tin để giải quyết chúng. Nếu bạn không thể tìm thấy mã lỗi cho lỗi triển khai của mình, hãy xem [Tìm mã lỗi](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Khắc phục sự cố lỗi triển khai](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Khắc phục sự cố di chuyển tài nguyên Azure sang nhóm tài nguyên mới hoặc đăng ký](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Lưu ý rằng nếu bạn muốn nâng cấp đăng ký Azure của mình, chẳng hạn như chuyển từ miễn phí sang thanh toán-như-bạn-đi, bạn sẽ cần phải chuyển đổi đăng ký của mình.

- Để nâng cấp bản dùng thử miễn phí, hãy xem [nâng cấp bản dùng thử miễn phí hoặc Microsoft sẽ tưởng tượng đăng ký Azure để thanh toán-như-bạn-đi](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Để thay đổi một tài khoản thanh toán-như-bạn-đi, hãy xem mục [thay đổi đăng ký Azure Pay-as-You-Go của bạn sang một ưu đãi khác nhau](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Để thêm hoặc liên kết một thuê bao Azure vào đối tượng thuê Azure Active Directory của bạn:**

1. Đăng nhập và chọn đăng ký mà bạn muốn sử dụng từ [trang đăng ký trong Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Chọn **thay đổi thư mục**.
3. Xem lại mọi cảnh báo xuất hiện, rồi chọn **thay đổi**.
4. Thư mục được thay đổi cho đăng ký và bạn sẽ nhận được thông báo thành công.
5. Sử dụng nút *thư mục* để đi đến thư mục mới của bạn. Có thể mất tối đa 10 phút để mọi thứ Hiển thị đúng cách.

**Tài liệu được đề xuất**

- [Chuyển quyền sở hữu của một thuê bao Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Di chuyển tài nguyên đến nhóm tài nguyên mới hoặc thuê bao](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Quản lý tài nguyên bằng Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
