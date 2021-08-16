---
title: Sự cố với Tài nguyên hoặc Tài nguyên Chính dịch vụ chính
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028098"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Sự cố với Tài nguyên hoặc Tài nguyên Chính dịch vụ chính

1. Nếu bạn vừa mới bắt đầu, đối tượng Chính của ứng dụng và dịch vụ trong [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) sẽ mô tả các đối tượng đăng ký ứng dụng, đối tượng ứng dụng và tên dịch vụ chính trong Azure Active Directory: chúng là gì, được dùng như thế nào và chúng có liên quan với nhau ra sao. Kịch bản ví dụ nhiều đối tượng thuê cũng được trình bày để minh họa mối quan hệ giữa đối tượng ứng dụng của ứng dụng và đối tượng chính của dịch vụ tương ứng.
2. Bạn có thể tìm hiểu thêm về mối quan hệ giữa ứng dụng và hiệu trưởng dịch vụ bằng cách đọc các ứng dụng và đối tượng chính của dịch [vụ Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Cách [thức:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Sử dụng cổng thông tin để tạo một ứng dụng và tài nguyên dịch vụ Azure AD chính có thể truy nhập tài nguyên sẽ hướng dẫn bạn cách tạo một ứng dụng và tài nguyên dịch vụ Azure Active Directory (Azure AD) mới, có thể được sử dụng với kiểm soát truy nhập dựa trên vai trò.
4. Với API chính [của dịch vụ, bạn](https://docs.microsoft.com/graph/api/resources/serviceprincipal)có thể quản lý theo chương trình các phiên bản của ứng dụng và kiểm soát những gì một ứng dụng có thể thực hiện trong đối tượng thuê của bạn.
5. [servicePrincipal resource type liệt](https://docs.microsoft.com/graph/api/resources/serviceprincipal) kê tất cả các thuộc tính và phương pháp cho loại tài nguyên servicePrincipal.
6. [Sự khác biệt về loại tài](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) nguyên giữa Azure AD Graph và Microsoft Graph làm nổi bật sự khác biệt giữa Azure AD Graph và Microsoft Graph nguyên. Nó hiển thị các tài nguyên có tên khác nhau hoặc không sẵn dùng; tài nguyên cũng nêu bật các tài nguyên sẵn có trong phiên bản beta của Microsoft Graph nhưng không có trong phiên bản v1.0.

**Sự cố với Người dùng Khách**

- [Khởi động nhanh:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Thêm người dùng khách vào thư mục của bạn trong cổng thông tin Azure cho bạn biết cách thêm người dùng khách mới vào thư mục Azure AD thông qua cổng thông tin Azure, gửi lời mời và xem giao diện quy trình quy đổi lời mời của người dùng khách.
- [Hướng dẫn: Tạo dòng người dùng Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) cho bạn biết cách tạo một số dòng người dùng được đề xuất bằng cách sử dụng cổng thông tin Azure. Nếu bạn đang tìm kiếm thông tin về cách thiết lập một dòng thông tin xác thực mật khẩu chủ sở hữu tài nguyên (ROPC) trong ứng dụng của bạn, hãy xem mục Đặt cấu hình dòng thông tin xác thực mật khẩu chủ sở hữu tài nguyên trong Azure AD B2C.
