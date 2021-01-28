---
title: Các vấn đề với yêu cầu và thuộc tính mã thông báo
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036082"
---
# <a name="issues-with-token-claims-and-attributes"></a>Các vấn đề với yêu cầu và thuộc tính mã thông báo

**Cập Nhật, cấu hình hoặc loại bỏ yêu cầu mã thông báo**

1. Bằng cách sử dụng Azure Active Directory (Azure AD), bạn có thể [tùy chỉnh kiểu yêu cầu bồi thường của vai trò](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) trong mã thông báo phản hồi mà bạn nhận được sau khi bạn ủy quyền cho một ứng dụng.
2. Các nhà phát triển ứng dụng có thể sử dụng các tuyên bố tùy chọn trong ứng dụng Azure AD của họ để xác định những tuyên bố mà họ muốn trong thẻ được gửi đến ứng dụng của họ. Để biết thêm thông tin, hãy xem [cung cấp tuyên bố tùy chọn vào ứng dụng của bạn](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Cấu hình tuyên bố nhóm cho các ứng dụng với Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Nếu dùng đăng nhập đơn seamless trong ứng dụng của bạn, hãy xem [tùy chỉnh tuyên bố phát hành trong các ứng dụng thông báo thông báo của doanh nghiệp SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Lập bản đồ thuộc tính tuyên bố**

1. Để cấu hình chính sách ánh xạ tuyên bố bằng PowerShell, hãy xem [tùy chỉnh tuyên bố phát ra bằng thẻ cho một ứng dụng cụ thể trong một đối tượng thuê (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Thuộc tính Schema của phần mở rộng thư mục cung cấp cách để lưu trữ dữ liệu bổ sung trong Azure Active Directory trên đối tượng người dùng và các đối tượng thư mục khác chẳng hạn như nhóm, chi tiết đối tượng thuê, hiệu trưởng dịch vụ. Chỉ các thuộc tính phần mở rộng trên đối tượng người dùng có thể được sử dụng để phát ra các yêu cầu cho các ứng dụng. [Sử dụng các thuộc tính phần mở rộng của sơ đồ trong thư mục trong yêu cầu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) mô tả cách sử dụng thuộc tính phần mở rộng sơ đồ danh mục để gửi dữ liệu người dùng đến các ứng dụng trong yêu cầu

Để biết thêm thông tin về các yêu cầu token, hãy xem:

- [Tuyên bố trong thẻ Access](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Khiếu nại trong một id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Tuyên bố](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) rằng bạn có thể trông đợi trong thẻ ID và thẻ Access do AZURE AD B2C phát hành
- [Tham khảo tuyên bố mã thông báo SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
