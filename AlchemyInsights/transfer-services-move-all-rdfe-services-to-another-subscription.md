---
title: Chuyển Dịch vụ - Di chuyển tất cả các dịch vụ RDFE sang một thuê bao khác
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940115"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Chuyển Dịch vụ - Di chuyển tất cả các dịch vụ RDFE sang một thuê bao khác

**Di chuyển tài nguyên**

Có thể di chuyển tài nguyên Azure sang một đăng ký Azure hoặc nhóm tài nguyên khác dưới cùng một đăng ký bằng cách sử dụng cổng thông tin Azure, Azure PowerShell, Azure CLI hoặc API REST để di chuyển tài nguyên.

Trước khi bạn có thể di chuyển tài nguyên, hãy xem:

- [Danh sách kiểm tra trước khi di chuyển tài nguyên](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Có thể di chuyển các dịch vụ](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cách xác thực việc di chuyển](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Hướng dẫn di chuyển về dịch vụ](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Để chuyển các tài nguyên hiện có sang nhóm tài nguyên hoặc đăng ký khác, bạn có thể sử dụng:

- [Cổng thông tin Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Hướng dẫn: [Di chuyển tài nguyên Azure sang một nhóm hoặc đăng ký tài nguyên khác](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Khắc phục lỗi với Trình quản lý Tài nguyên Azure**

Hãy tham khảo các bài viết dưới đây để tìm hiểu về một số lỗi triển khai Azure phổ biến và nhận thông tin để giải quyết các lỗi đó. Nếu bạn không thể tìm thấy mã lỗi cho lỗi triển khai của mình, hãy [xem mục Tìm mã lỗi](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Khắc phục lỗi triển khai](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Khắc phục sự cố di chuyển tài nguyên Azure sang nhóm hoặc đăng ký tài nguyên mới](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Lưu ý rằng nếu bạn muốn nâng cấp đăng ký Azure, chẳng hạn như chuyển đổi từ miễn phí sang thanh toán khi cần, bạn sẽ cần chuyển đổi đăng ký của mình.

- Để nâng cấp bản dùng thử miễn phí, hãy xem mục Nâng cấp bản dùng thử Miễn phí của bạn hoặc đăng ký [Microsoft Imagine Azure lên Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Để thay đổi tài khoản thanh toán khi cần, hãy xem mục Thay đổi đăng ký [Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)của bạn thành một ưu đãi khác.

**Để thêm hoặc liên kết đăng ký Azure với đối tượng thuê Azure Active Directory bạn:**

1. Đăng nhập và chọn đăng ký bạn muốn sử dụng từ trang [Đăng ký trong cổng thông tin Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Chọn Thay **đổi thư mục**.
3. Xem lại mọi cảnh báo xuất hiện, rồi chọn Thay **đổi**.
4. Thư mục được thay đổi cho đăng ký và bạn sẽ nhận được thông báo thành công.
5. Sử dụng *bộ chuyển* đổi Thư mục để đi đến thư mục mới của bạn. Có thể mất đến 10 phút để mọi thứ hiển thị đúng cách.

**Tài liệu được Đề xuất**

- [Chuyển quyền sở hữu đăng ký Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Di chuyển tài nguyên sang nhóm tài nguyên hoặc đăng ký mới](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Quản lý tài nguyên bằng cổng thông tin Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
