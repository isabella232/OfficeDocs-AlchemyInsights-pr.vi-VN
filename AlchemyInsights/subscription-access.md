---
title: Quyền truy nhập đăng ký
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999262"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Không thể đăng nhập Azure do sự cố trình duyệt (Trình duyệt bị treo, tiếp tục quay xoay, không tải, v.v.)

Bạn có thể bị ảnh hưởng bởi sự mất điện. Vui lòng kiểm tra xem có sự cố nào đang diễn ra không: Trạng [thái Azure Health](https://status.azure.com/status/history/).

Vui lòng đăng xuất khỏi tất cả các phiên Azure hiện hoạt. Bắt đầu chế độ riêng tư hoặc ẩn danh của trình duyệt web.

Bạn cũng có thể thử Làm mới trình duyệt, sử dụng một trình duyệt khác, xóa cookie bộ đệm ẩn nếu cách trên không hiệu quả.

Tìm hiểu thêm: [Khắc phục sự cố đăng nhập](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Không thể truy nhập đăng ký**

Trong cổng [thông tin Azure](https://portal.azure.com/), hãy đảm bảo chọn đúng thư mục Azure từ tài khoản ở trên cùng bên phải.

Trong Trung tâm [Tài khoản Azure](https://account.windowsazure.com/Subscriptions), hãy đảm bảo tài khoản được sử dụng có phải là người quản trị tài khoản hay không.

Tìm hiểu thêm: Tìm [thấy Khắc phục Sự cố Không tìm thấy Gói đăng ký](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Không thể truy nhập lịch sử thanh toán**

Người quản trị tài khoản cần đảm bảo rằng người dùng truy nhập thông tin thanh toán được thêm vào Azure Active directory với tư cách là người dùng khách: Thêm hoặc xóa [người dùng mới.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Sau đó, người dùng cần được trao vai trò Người quản trị toàn cục: [Gán vai trò cho người dùng.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Đăng bài viết này, người dùng có thể được cấp quyền truy nhập thanh toán bằng các chính sách RBAC: [Cấp quyền truy nhập vào thanh toán.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tài liệu được Đề xuất**

-   [Tôi không thể đăng nhập để quản lý đăng ký Azure của mình](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)