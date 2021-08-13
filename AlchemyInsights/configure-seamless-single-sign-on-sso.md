---
title: Đặt cấu hình Đăng nhập Đơn Liền mạch (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966059"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Đặt cấu hình Đăng nhập Đơn Liền mạch (SSO)

**Đặt cấu hình Ứng dụng**

1. Bạn sẽ nhận được các giá trị từ nhà cung cấp ứng dụng. Bạn có thể nhập thủ công các giá trị hoặc tải lên tệp siêu dữ liệu để trích xuất giá trị của các trường.
2. Nhiều ứng dụng đã được đặt cấu hình sẵn để hoạt động với Azure AD. Những ứng dụng này được liệt kê trong bộ sưu tập ứng dụng mà bạn có thể duyệt khi thêm ứng dụng vào đối tượng thuê Azure AD của mình. Chuỗi [bắt đầu nhanh sẽ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) hướng dẫn bạn toàn bộ quy trình.
3. Để tạo một ứng dụng không phải là bộ sưu tập, bạn có thể bấm **vào + Tạo** nút Ứng dụng của riêng bạn và đặt tên cho Ứng dụng của bạn.
    - Theo mặc định, ứng dụng này **sẽ** chọn Tích hợp bất kỳ ứng dụng nào khác mà bạn không tìm thấy trong bộ sưu tập, đây là tùy chọn phù hợp cho các ứng dụng Không phải bộ sưu tập.
    - Sau khi nhấn **tạo sau** khi đặt tên cho ứng dụng, ứng dụng sẽ tạo một Ứng dụng Doanh nghiệp không phải bộ sưu tập mới.
    - Sau đó, bạn  có thể  dẫn hướng đến Đăng nhập Đơn trong Quản lý ứng dụng đó và sẽ có thể thấy các kỹ thuật khác nhau để triển khai ứng dụng trong môi trường của bạn.

**Đặt cấu hình Seamless SSO cho một ứng dụng cụ thể**

Đối với các ứng dụng trong bộ sưu tập, bạn sẽ tìm thấy hướng dẫn chi tiết, từng bước. Để truy nhập các bước, bạn có thể duyệt danh sách tất cả các hướng dẫn cấu hình ứng dụng tại hướng dẫn [cấu hình ứng dụng SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Đặt cấu hình SSO dựa trên SAML**

1. Khởi động Nhanh: Thiết lập đăng nhập đơn (SSO) dựa trên SAML cho ứng dụng trong đối tượng [thuê Azure Active Directory (Azure AD) của bạn.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Để tìm hiểu thêm về tùy chọn dựa trên SAML dành cho đăng nhập đơn, hãy xem mục Hiểu rõ đăng [nhập đơn dựa trên SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Để tìm hiểu về các yêu cầu và phản hồi xác thực SAML 2.0 mà Azure Active Directory (Azure AD) hỗ trợ cho Sign-On đơn (SSO), hãy xem giao thức [SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)Sign-On đơn.
4. Để tìm hiểu cách tạo và đặt cấu hình đăng nhập đơn dựa trên SAML (SSO) cho ứng dụng của bạn trong Azure Active Directory (Azure AD) bằng cách sử dụng API Microsoft Graph, hãy xem mục Đặt cấu hình đăng nhập đơn dựa trên [SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)cho ứng dụng của bạn bằng cách sử dụng API Microsoft Graph .
5. Để tìm hiểu cách Azure AD sử dụng giao thức SAML, hãy [xem mục Cách thức Nền tảng định danh Microsoft sử dụng giao thức SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Đặt cấu hình Mã thông báo và Yêu cầu**

1. [Cách: tùy chỉnh các yêu cầu được phát hành trong mã thông báo SAML cho các ứng dụng doanh nghiệp](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Để tìm hiểu cách đặt cấu hình yêu cầu bằng PowerShell, hãy xem Cách thức: Tùy chỉnh các khiếu nại được làm rỗng trong mã thông báo cho một ứng dụng cụ thể trong một đối tượng [thuê (Bản xem trước).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Để tìm hiểu cách đặt cấu hình yêu cầu tùy chọn, hãy [xem Cách thức: Cung cấp yêu cầu tùy chọn cho ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Để tìm hiểu cách sử dụng thuộc tính phần mở rộng sơ đồ thư mục để gửi dữ liệu người dùng đến các ứng dụng trong yêu cầu mã thông báo, hãy xem Sử dụng thuộc tính phần mở rộng sơ đồ thư mục trong [tuyên bố.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Để tìm hiểu cách đặt cấu hình thời hạn mã thông báo, hãy xem Thời hạn mã thông báo có thể cấu hình [trong Nền tảng định danh Microsoft (bản xem trước).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Đặt cấu hình](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) chính sách thời hạn mã thông báo (bản xem trước) - Trong bài viết này, chúng tôi sẽ đi qua một kịch bản chính sách phổ biến có thể giúp bạn đưa ra các quy tắc mới cho thời hạn mã thông báo. Trong ví dụ này, bạn sẽ tìm hiểu cách tạo chính sách yêu cầu người dùng xác thực thường xuyên hơn trong ứng dụng web của bạn.

**Khắc phục sự cố về Cấu hình SSO**

- Để biết các câu hỏi thường gặp về Azure Active Directory Seamless Single Sign-On (Seamless SSO), hãy xem [Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Để biết thông tin về các sự cố phổ biến về Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), xem mục Khắc [phục sự cố Azure Active Directory Đăng](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)nhập Một lần Liền mạch .
