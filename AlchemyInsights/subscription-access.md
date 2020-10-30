---
title: Truy nhập thuê bao
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807727"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Không thể đăng nhập Azure do các sự cố của trình duyệt (trình duyệt bị treo, Giữ quay, không tải, v.v.)

Bạn có thể bị ảnh hưởng bởi sự mất điện. Vui lòng kiểm tra xem liệu có đang mất liên tục không: [Azure trạng thái tình trạng](https://status.azure.com/status/history/).

Vui lòng đăng xuất khỏi tất cả các phiên họp Azure hiện hoạt. Bắt đầu chế độ một cách riêng tư hoặc ẩn danh trong trình duyệt web của bạn.

Bạn cũng có thể thử làm mới trình duyệt, sử dụng trình duyệt khác, xóa cookie bộ đệm ẩn nếu ở trên không hoạt động.

Tìm hiểu thêm: [khắc phục sự cố đăng nhập](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Không thể truy nhập đăng ký**

Trong [cổng thông tin Azure](https://portal.azure.com/), hãy đảm bảo rằng thư mục Azure đúng được chọn từ tài khoản ở phía trên cùng bên phải.

Trong [Trung tâm tài khoản Azure](https://account.windowsazure.com/Subscriptions), hãy đảm bảo rằng nếu tài khoản được sử dụng là người quản trị tài khoản.

Tìm hiểu thêm: [khắc phục sự cố không tìm thấy đăng ký](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Không thể truy nhập lịch sử thanh toán**

Người quản trị tài khoản cần phải đảm bảo rằng người dùng truy nhập thông tin thanh toán sẽ được thêm vào trong thư mục Azure Active Directory với tư cách là người dùng khách: [Thêm hoặc xóa người dùng mới](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Người dùng sau đó cần có vai trò quản trị toàn cầu: [gán vai trò cho người dùng](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Đăng bài này, người dùng có thể được truy nhập thanh toán bằng cách sử dụng chính sách RBAC: [cấp quyền truy nhập vào thanh toán](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tài liệu được đề xuất**

-   [Tôi không thể đăng nhập để quản lý đăng ký Azure của tôi](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)