---
title: Quyền API và quy trình chấp thuận
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405446"
---
# <a name="api-permissions-and-consent-process"></a>Quyền API và quy trình chấp thuận

Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận. [Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph. Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.

**Thiết lập hoặc Cập Nhật hiệu trưởng dịch vụ**

- [Tạo hiệu trưởng](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) -bài viết này cho bạn biết cách tạo đối tượng dịch vụ mới.
- [Tạo một AZURE AD app & dịch vụ chính trong cổng thông tin](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) -bài viết này cho bạn biết cách tạo ứng dụng Azure Active Directory (Azure AD) và hiệu trưởng dịch vụ có thể được sử dụng với điều khiển truy nhập dựa trên vai trò.
- Các [ứng dụng & hiệu trưởng dịch vụ trong AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) -bài viết này mô tả đăng ký ứng dụng, đối tượng ứng dụng và hiệu trưởng dịch vụ trong Azure Active Directory: chúng là gì, cách chúng được dùng và cách chúng liên quan đến nhau.

**Thêm hoặc cập nhật đăng ký ứng dụng và cung cấp sự đồng ý của người quản trị**

- [Tạo đăng ký ứng dụng](https://docs.microsoft.com/graph/api/application-post-applications) -bài viết này cho bạn biết cách tạo đối tượng ứng dụng mới.
- [Cập Nhật đăng ký ứng dụng-quyền API](https://docs.microsoft.com/graph/api/application-update) -bài viết này cho bạn biết cách cập nhật các thuộc tính của đối tượng ứng dụng.
- [Cung cấp sự chấp thuận quản trị](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) -chấp thuận và đồng ý người quản trị trong chung, chúng tôi yêu cầu người quản trị được cấp phép một cách rõ ràng.
- Hàm [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) -bộ chứa quản lý vai trò cho các định nghĩa vai trò hợp nhất và gán vai trò cho các nhà cung cấp Microsoft 365 RBAC hỗ trợ nhiều hiệu trưởng và nhiều phạm vi trong một nhiệm vụ vai trò duy nhất. Điều này khác với loại tài nguyên *Rbacapplication* . Microsoft InTune là một ví dụ về một nhà cung cấp RBAC như vậy. Gán vai trò trong InTune có thể có một mảng hiệu trưởng và một mảng của các nhóm phạm vi. **Đây là trong phiên bản beta, có nghĩa là nó vẫn đang được phát triển và không được khuyên dùng để sử dụng trong sản xuất.**
