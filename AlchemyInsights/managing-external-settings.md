---
title: Quản lý thiết đặt bên ngoài
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294428"
---
# <a name="managing-external-settings"></a>Quản lý thiết đặt bên ngoài

**Thông báo**

- [Deprecation của WebView hỗ trợ đăng nhập từ Google bắt đầu từ 4 tháng 1, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support). Kiểm tra xem ứng dụng của bạn có bị ảnh hưởng bằng cách theo dõi hướng dẫn của Google trên tính tương thích kiểm tra không
- Đảm bảo sử dụng WebView System hoặc trình duyệt hệ thống khi đăng nhập vào người dùng của bạn với tài khoản Google dành cho người dùng

**Quản lý thiết đặt lời mời**

Xác nhận rằng bạn đã [cấu hình các thiết đặt cộng tác bên ngoài](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) để cho phép những người thích hợp gửi thư mời.

**Quản lý quyền truy nhập của người dùng khách**

1. Người quản trị toàn cầu có thể quản lý quyền truy nhập của khách trong thư mục qua cổng thông tin Azure bằng cách cấu hình quyền truy nhập của khách trên trang thiết đặt cộng tác bên ngoài. [Tìm hiểu thêm về thiết đặt này](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).
2. Nếu bạn muốn khách của mình truy nhập vào các ứng dụng như nhóm hoặc SharePoint, hãy xác nhận rằng bạn đã cấu hình những ứng dụng này để cho phép truy nhập của khách. Tìm hiểu thêm về các [thiết đặt nhóm](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) và [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).

**Cấu hình thư mời:**

- [Bật cộng tác bên ngoài B2B và quản lý những người có thể mời khách](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cho phép hoặc chặn thư mời cho người dùng từ các tổ chức cụ thể](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Cấu hình các nhà cung cấp căn cước được phép:**

- [Liên kết Google](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Liên kết trực tiếp](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Xác thực mật mã một lần email](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
