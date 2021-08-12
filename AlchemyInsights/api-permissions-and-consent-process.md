---
title: Quy trình Cấp phép và Chấp thuận API
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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932083"
---
# <a name="api-permissions-and-consent-process"></a>Quy trình Cấp phép và Chấp thuận API

Để ứng dụng của bạn truy nhập dữ liệu trong Microsoft Graph, người dùng hoặc người quản trị phải cấp đúng quyền thông qua một quy trình đồng ý. [Microsoft Graph chiếu quyền sẽ](https://docs.microsoft.com/graph/permissions-reference) liệt kê các quyền liên kết với mỗi tập hợp API chính Graph Microsoft. Tài liệu cũng cung cấp hướng dẫn về cách sử dụng các quyền.

**Thiết lập hoặc cập nhật tài liệu chính của dịch vụ**

- [Tạo serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Bài viết này cho bạn biết cách tạo đối tượng servicePrincipal mới.
- Tạo một ứng dụng [Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) chính của dịch vụ trong cổng thông tin - Bài viết này cho bạn biết cách tạo một ứng dụng và tài khoản dịch vụ Azure Active Directory (Azure AD) mới có thể được sử dụng với kiểm soát truy nhập dựa trên vai trò.
- Ứng dụng & chính của dịch vụ trong [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - Bài viết này mô tả việc đăng ký ứng dụng, đối tượng ứng dụng và tên dịch vụ chính trong Azure Active Directory: chúng là gì, được sử dụng như thế nào và chúng có liên quan với nhau ra sao.

**Thêm hoặc cập nhật đăng ký ứng dụng và cung cấp sự chấp thuận của người quản trị**

- [Tạo đăng ký ứng dụng](https://docs.microsoft.com/graph/api/application-post-applications) - Bài viết này cho bạn biết cách tạo đối tượng ứng dụng mới.
- [Cập nhật đăng ký ứng dụng - Quyền API](https://docs.microsoft.com/graph/api/application-update) - Bài viết này cho bạn biết cách cập nhật thuộc tính của đối tượng ứng dụng.
- [Đưa ra sự chấp thuận](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) của người quản trị - Đối với sự chấp thuận và đồng ý của người quản trị nói chung, chúng tôi yêu cầu người quản trị chấp thuận một cách rõ ràng.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Bộ chứa quản lý vai trò cho định nghĩa vai trò hợp nhất và gán vai trò cho nhà cung cấp Microsoft 365 RBAC hỗ trợ nhiều hiệu trưởng và nhiều phạm vi trong một lần gán vai trò duy nhất. Điều này khác với *loại tài nguyên rbacApplication.* Microsoft Intune là một ví dụ về nhà cung cấp RBAC. Chỉ định vai trò trong Intune có thể có một mảng hiệu trưởng và một mảng các nhóm phạm vi. **Điều này ở bản beta, có nghĩa là nó vẫn đang trong giai đoạn phát triển và không được khuyến nghị sử dụng trong sản xuất.**
