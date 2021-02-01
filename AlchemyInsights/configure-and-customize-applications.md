---
title: Cấu hình và tùy chỉnh các ứng dụng
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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063714"
---
# <a name="configure-and-customize-applications"></a>Cấu hình và tùy chỉnh các ứng dụng

**Cấu hình ứng dụng**

1. [Bắt đầu nhanh: cấu hình các thuộc tính cho một ứng dụng trong công việc Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) cho bạn biết cách cấu hình một số thuộc tính cho một ứng dụng.
2. Để giúp tích hợp các ứng dụng của bạn với Azure Active Directory, chúng tôi đã phát triển [một tuyển tập các hướng dẫn hướng dẫn](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) bạn qua cấu hình.
3. [Làm thế nào để cấu hình ứng dụng proxy ứng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) dụng giúp bạn tìm hiểu cách cấu hình ứng dụng proxy ứng dụng trong Azure AD để hiển thị các ứng dụng tại chỗ của bạn vào điện toán đám mây.
4. [Tải về pingaccess và cấu hình ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): làm theo các hướng dẫn trong *đặt cấu hình Pingaccess cho Azure AD để bảo vệ các ứng dụng* được phát hành bằng Microsoft Azure AD Application proxy on the ping Identity web site và tải xuống phiên bản mới nhất của pingaccess.

**Lỗi ứng dụng đã cấu hình sai (AADSTS650056)**

1. Đảm bảo bạn đang truy nhập vào ứng dụng từ địa chỉ đăng nhập do chủ sở hữu ứng dụng cung cấp. Nếu không, hãy đăng nhập vào ứng dụng thông qua quy trình bình thường của nó. Trong hầu hết các trường hợp, điều này sẽ tự động giải quyết tự nhiên. Nếu không, thì bài đăng này có thể giúp khắc phục sự cố và giải quyết.
2. **Nếu tổ chức của bạn sở hữu ứng dụng** (có nghĩa là đăng ký ứng dụng nằm trong tổ chức của bạn):
    - Tối thiểu, chúng tôi đề xuất `User.Read` quyền hoặc được `openid` ủy quyền từ **Microsoft graph** được thêm vào.
    - Đảm bảo ứng dụng và tất cả các quyền của nó được đồng ý với. Bạn có thể xác nhận điều này bằng cách nhìn vào cột **trạng thái** của đăng ký ứng dụng bên trong **API quyền**.
    - Trong một số kịch bản, ứng dụng có thể là bên thứ ba có thể được đăng ký trong tổ chức của bạn. Xác nhận nếu ứng dụng này được liệt kê trong đăng ký ứng dụng của bạn (không phải ứng dụng doanh nghiệp).
    - Nếu bạn tiếp tục thấy thông báo lỗi này. Sau đó, bạn có thể cần phải xây dựng URL chấp thuận được mô tả ở **bước 4**.
3. **Nếu tổ chức của bạn không phải là chủ sở hữu ứng dụng và dùng nó như một ứng dụng của bên thứ ba**:
    - Nếu bạn là người quản trị toàn cầu/công ty, bạn sẽ thấy màn hình chấp thuận. Hãy đảm bảo rằng bạn đánh dấu **vào hộp "chấp thuận thay mặt cho tổ chức của bạn"**.
    - Nếu bạn không nhìn thấy màn hình chấp thuận, hãy xóa ứng dụng Enterprise, rồi thử lại.
    - Nếu bạn tiếp tục thấy thông báo lỗi này. Sau đó, bạn có thể cần phải xây dựng URL chấp thuận được mô tả ở **bước 4**.
4. Việc **xây dựng URL chấp thuận được dùng theo cách thủ công**: Nếu ứng dụng được thiết kế để truy nhập vào một tài nguyên cụ thể, bạn có thể không sử dụng các nút chấp thuận từ cổng thông tin Azure, bạn sẽ cần phải tự tạo URL chấp thuận của riêng bạn và sử dụng điều này.
    - Bạn sẽ cần lấy `{App-Id}` và `{App-Uri-Id}` từ chủ sở hữu ứng dụng. `{Tenant-Id}` sẽ là mã định danh đối tượng thuê của bạn. Điều này sẽ có `yourdomain.onmicrosoft.com` hoặc ID thư mục của bạn.
    - Nếu ứng dụng đang truy nhập chính nó cho tài nguyên, thì `{App-Id}` và `{App-Uri-Id}` sẽ giống như vậy.
5. Để biết thêm thông tin, hãy xem mục các [vấn đề đăng nhập vào các ứng dụng được đặt cấu hình đăng nhập vào SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Tùy chỉnh ứng dụng**

- [Thêm thương hiệu vào trang đăng nhập Azure Active Directory của tổ chức của bạn](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) -dùng logo của tổ chức bạn và các lược đồ màu tùy chỉnh để cung cấp một giao diện nhất quán cho các trang đăng nhập Azure Active Directory (Azure AD) của bạn.
- [Thêm tên miền tùy chỉnh của bạn bằng cổng thông tin Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) -mọi đối tượng thuê Azure AD mới đi kèm với tên miền ban đầu. Bạn không thể thay đổi hoặc xóa tên miền ban đầu, nhưng bạn có thể thêm tên của tổ chức của mình. Thêm tên miền tùy chỉnh giúp bạn tạo tên người dùng quen thuộc với người dùng của bạn.
