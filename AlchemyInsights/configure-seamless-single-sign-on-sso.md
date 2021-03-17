---
title: Đặt cấu hình đăng nhập đơn (SSO) liền mạch
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841667"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Đặt cấu hình đăng nhập đơn (SSO) liền mạch

**Cấu hình ứng dụng**

1. Bạn sẽ nhận được các giá trị từ nhà cung cấp ứng dụng. Bạn có thể nhập thủ công các giá trị hoặc tải lên một tệp siêu dữ liệu để trích xuất giá trị của các trường.
2. Nhiều ứng dụng đã được cấu hình sẵn để làm việc với Azure AD. Những ứng dụng này được liệt kê trong bộ sưu tập các ứng dụng mà bạn có thể duyệt khi bạn thêm ứng dụng vào đối tượng thuê Azure AD của bạn. [Chuỗi bắt đầu nhanh chóng](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) hướng dẫn bạn qua quy trình.
3. Để tạo ứng dụng không phải là bộ sưu tập, bạn có thể bấm vào **+ tạo nút ứng dụng riêng của bạn** và đặt tên cho ứng dụng của bạn.
    - Theo mặc định, nó sẽ chọn **tích hợp bất kỳ ứng dụng nào khác mà bạn không tìm thấy trong bộ sưu tập** là tùy chọn đúng đối với các ứng dụng không phải bộ sưu tập.
    - Sau khi bạn nhấn **tạo** tên sau khi đặt tên cho ứng dụng, nó sẽ tạo một ứng dụng doanh nghiệp không phải là bộ sưu tập mới.
    - Sau đó, bạn có thể dẫn hướng đến **đăng nhập đơn** bên dưới **quản lý** ứng dụng đó và bạn sẽ có thể thấy các kỹ thuật khác nhau để thực hiện nó trong môi trường của bạn.

**Cấu hình SSO liền mạch cho một ứng dụng cụ thể**

Đối với các ứng dụng trong bộ sưu tập, bạn sẽ tìm thấy chi tiết, hướng dẫn từng bước. Để truy nhập các bước bạn có thể duyệt danh sách tất cả các hướng dẫn cấu hình ứng dụng tại [hướng dẫn cấu hình ứng dụng Saas](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Cấu hình SSO dựa trên SAML**

1. [Bắt đầu nhanh: thiết lập đăng nhập đơn (SSO) SAML cho một ứng dụng trong đối tượng thuê Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Để tìm hiểu thêm về tùy chọn dựa trên SAML cho đăng nhập một lần, hãy xem tìm [hiểu đăng nhập đơn dựa trên SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Để tìm hiểu về các yêu cầu xác thực SAML 2,0 và phản hồi mà Azure Active Directory (Azure AD) hỗ trợ cho Sign-On đơn (SSO), hãy xem [giao thức Sign-On SAML đơn](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Để tìm hiểu cách tạo và cấu hình đăng nhập đơn (SSO) SAML cho ứng dụng của bạn trong Azure Active Directory (Azure AD) bằng cách sử dụng Microsoft graph API, hãy xem [cấu hình đăng nhập đơn dựa trên SAML cho ứng dụng của bạn bằng cách sử dụng Microsoft GRAPH API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Để tìm hiểu cách Azure AD sử dụng giao thức SAML, hãy xem [cách nền tảng định danh Microsoft sử dụng giao thức SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Cấu hình thẻ và tuyên bố**

1. [Cách: tùy chỉnh tuyên bố phát hành trong các ứng dụng của mã thông báo SAML cho doanh nghiệp](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Để tìm hiểu cách đặt cấu hình khiếu nại bằng PowerShell, hãy xem [làm thế nào để: tùy chỉnh tuyên bố phát ra trong thẻ cho một ứng dụng cụ thể trong một đối tượng thuê (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Để tìm hiểu cách đặt cấu hình tuyên bố tùy chọn, hãy xem [cách: cung cấp tuyên bố tùy chọn vào ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Để tìm hiểu cách sử dụng thuộc tính phần mở rộng sơ đồ của thư mục để gửi dữ liệu người dùng đến các ứng dụng trong yêu cầu mã thông báo, hãy xem [mục sử dụng thuộc tính phần mở rộng của sơ đồ trong khiếu nại](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Để tìm hiểu cách đặt cấu hình hạn token, hãy xem [cấu hình hạn token trong Microsoft Identity Platform (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Cấu hình chính sách Lifetime token (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -trong bài viết này, chúng tôi hướng dẫn thông qua một tình huống chính sách phổ biến có thể giúp bạn áp đặt các quy tắc mới cho tuổi thọ mã thông báo. Trong ví dụ này, bạn sẽ tìm hiểu cách tạo chính sách yêu cầu người dùng xác thực thường xuyên hơn trong ứng dụng web của bạn.

**Khắc phục sự cố cấu hình SSO**

- Đối với các câu hỏi thường gặp về Azure Active Directory seamless Sign-On đơn (SSO liền mạch), hãy xem [Azure Active Directory liền mạch Single đăng nhập: câu hỏi thường gặp](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Để biết thông tin khắc phục sự cố về các vấn đề thường gặp về Azure Active Directory (Azure AD) Sign-On một lần duy nhất (không liền mạch SSO), hãy xem [khắc phục sự cố Azure Active Directory liền mạch Single đăng nhập](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
