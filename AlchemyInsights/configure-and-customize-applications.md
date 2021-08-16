---
title: Đặt cấu hình và tùy chỉnh ứng dụng
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045010"
---
# <a name="configure-and-customize-applications"></a>Đặt cấu hình và tùy chỉnh ứng dụng

**Đặt cấu hình Ứng dụng**

1. [Khởi động nhanh: Đặt cấu](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) hình thuộc tính cho một ứng dụng trong đối tượng thuê Azure Active Directory (Azure AD) của bạn cho bạn biết cách đặt cấu hình một số thuộc tính cho một ứng dụng.
2. Để giúp tích hợp ứng dụng của bạn Azure Active Directory, chúng tôi đã phát triển một [tập hợp](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) các hướng dẫn hướng dẫn giúp bạn thực hiện cấu hình.
3. [Làm thế nào](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) để cấu hình một ứng dụng Proxy Ứng dụng sẽ giúp bạn hiểu cách cấu hình một ứng dụng Proxy Ứng dụng bên trong Azure AD để hiển thị các ứng dụng tại chỗ của bạn lên đám mây.
4. Tải xuống [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)và đặt cấu hình ứng dụng của bạn: Làm theo các hướng dẫn trong mục Đặt cấu hình *PingAccess* cho Azure AD để bảo vệ các ứng dụng đã phát hành bằng Microsoft Azure AD Application Proxy trên website Định danh Ping và tải xuống phiên bản mới nhất của PingAccess.

**Lỗi Ứng dụng Cấu hình Sai (AADSTS650056)**

1. Đảm bảo rằng bạn đang truy nhập vào ứng dụng từ địa chỉ đăng nhập do chủ sở hữu ứng dụng cung cấp. Nếu không có nghĩa là đăng nhập vào ứng dụng thông qua quy trình bình thường. Trong hầu hết các trường hợp, quá trình này sẽ tự động giải quyết một cách tự động. Nếu không, bài đăng này có thể giúp khắc phục sự cố và giải quyết vấn đề.
2. **Nếu tổ chức của bạn sở hữu ứng dụng (có** nghĩa là đăng ký ứng dụng thuộc tổ chức của bạn):
    - Tối thiểu, chúng tôi đề xuất `User.Read` quyền ủy nhiệm từ Microsoft `openid` **Graph** được thêm vào.
    - Đảm bảo ứng dụng và tất cả các quyền của ứng dụng được chấp thuận. Bạn có thể xác minh điều này bằng cách xem cột **Trạng** thái của Đăng ký ứng dụng trong **Quyền API.**
    - Trong một số kịch bản, ứng dụng có thể là bên thứ ba tuy nhiên nó có thể được đăng ký trong tổ chức của bạn. Xác nhận liệu ứng dụng này có được liệt kê trong đăng ký Ứng dụng của bạn hay không (không phải ứng dụng Doanh nghiệp).
    - Nếu bạn tiếp tục thấy thông báo lỗi này. Sau đó, có thể bạn cần xây dựng URL đồng ý được mô **tả ở bước 4.**
3. **Nếu tổ chức của bạn không phải là chủ sở hữu ứng dụng và sử dụng ứng dụng đó làm ứng dụng bên thứ ba:**
    - Nếu bạn là người quản trị Toàn cầu/Công ty, bạn sẽ thấy màn hình đồng ý. Đảm bảo bạn đánh dấu vào hộp **"Đồng ý thay mặt cho tổ chức của bạn".**
    - Nếu bạn không thấy màn hình đồng ý, hãy xóa ứng dụng Doanh nghiệp rồi thử lại.
    - Nếu bạn tiếp tục thấy thông báo lỗi này. Sau đó, có thể bạn cần xây dựng URL đồng ý được mô **tả ở bước 4.**
4. Xây dựng **URL** đồng ý theo cách thủ công để sử dụng: Nếu ứng dụng được thiết kế để truy nhập một tài nguyên cụ thể, bạn có thể không sử dụng được các nút Đồng ý từ cổng thông tin Azure, bạn sẽ cần phải tạo thủ công URL đồng ý của riêng mình và sử dụng url này.
    - Bạn sẽ cần phải có được và `{App-Id}` từ chủ sở hữu ứng `{App-Uri-Id}` dụng. `{Tenant-Id}` sẽ là mã định danh đối tượng thuê của bạn. Đây sẽ là ID `yourdomain.onmicrosoft.com` thư mục của bạn.
    - Nếu ứng dụng đang truy nhập chính nó cho tài nguyên thì `{App-Id}` sau đó, `{App-Uri-Id}` và sẽ giống nhau.
5. Để biết thêm thông tin, hãy xem mục Các sự cố khi đăng nhập vào ứng dụng được đặt [cấu hình đăng nhập một lần dựa trên SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Tùy chỉnh Ứng dụng**

- Thêm thương hiệu vào trang đăng nhập [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) của tổ chức bạn - Sử dụng logo và bảng phối màu tùy chỉnh của tổ chức để mang đến giao diện nhất quán cho các trang đăng nhập Azure Active Directory (Azure AD) của bạn.
- [Thêm tên miền riêng của bạn bằng cổng thông tin Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - Mỗi đối tượng thuê Azure AD mới đều có tên miền ban đầu. Bạn không thể thay đổi hoặc xóa tên miền ban đầu, nhưng bạn có thể thêm tên của tổ chức mình. Việc thêm tên miền riêng sẽ giúp bạn tạo ra các tên người dùng quen thuộc với người dùng của mình.
