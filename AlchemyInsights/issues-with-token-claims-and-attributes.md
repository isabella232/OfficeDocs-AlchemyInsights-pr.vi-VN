---
title: Sự cố với Yêu cầu Mã thông báo và Thuộc tính
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012906"
---
# <a name="issues-with-token-claims-and-attributes"></a>Sự cố với Yêu cầu Mã thông báo và Thuộc tính

**Cập nhật, cấu hình hoặc loại bỏ yêu cầu mã thông báo**

1. Bằng cách sử Azure Active Directory (Azure AD), bạn có thể tùy chỉnh loại khiếu nại cho vai trò yêu cầu trong mã thông báo phản hồi mà bạn nhận được sau khi ủy quyền một ứng dụng. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. Các nhà phát triển ứng dụng có thể sử dụng các khiếu nại không bắt buộc trong ứng dụng Azure AD của mình để chỉ định những yêu cầu họ muốn có trong mã thông báo được gửi tới ứng dụng của mình. Để biết thêm thông tin, hãy [xem phần Cung cấp yêu cầu tùy chọn cho ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Đặt cấu hình yêu cầu nhóm cho các ứng dụng Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Nếu sử dụng Đăng nhập Đơn Liền mạch trong ứng dụng của bạn, hãy xem các yêu cầu tùy chỉnh được đưa ra trong mã thông báo [SAML cho các ứng dụng doanh nghiệp.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Ánh xạ Thuộc tính Yêu cầu**

1. Để cấu hình chính sách ánh xạ tuyên bố bằng PowerShell, hãy xem Tùy chỉnh các yêu cầu được làm rỗng trong các mã thông báo cho một ứng dụng cụ thể trong đối tượng [thuê (Bản xem trước).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Thuộc tính phần mở rộng sơ đồ thư mục cung cấp cách lưu trữ dữ liệu bổ sung trong Azure Active Directory đối tượng người dùng và các đối tượng thư mục khác như nhóm, chi tiết đối tượng thuê, tên dịch vụ chính. Chỉ có thể sử dụng thuộc tính phần mở rộng trên đối tượng người dùng để làm rỗng các khiếu nại đối với ứng dụng. [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.

Để biết thêm thông tin về yêu cầu mã thông báo, hãy xem:

- [Yêu cầu trong mã thông báo truy nhập](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Yêu cầu trong một id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Tuyên bố rằng](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) bạn có thể mong đợi trong mã thông báo ID và mã thông báo truy nhập do Azure AD B2C phát hành
- [Tham chiếu yêu cầu mã thông báo SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
