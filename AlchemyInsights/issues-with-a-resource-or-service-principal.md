---
title: Các vấn đề với tài nguyên hoặc hiệu trưởng dịch vụ
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714465"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Các vấn đề với tài nguyên hoặc hiệu trưởng dịch vụ

1. Nếu bạn chỉ bắt đầu, [ứng dụng và dịch vụ đối tượng chính trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) mô tả đăng ký ứng dụng, đối tượng ứng dụng và hiệu trưởng dịch vụ trong Azure Active Directory: chúng là gì, cách chúng được dùng và cách chúng liên quan đến nhau. Một kịch bản ví dụ đa người thuê cũng được trình bày để minh họa mối quan hệ giữa đối tượng ứng dụng của ứng dụng và đối tượng chính Dịch vụ tương ứng.
2. Bạn có thể tìm hiểu thêm về mối quan hệ giữa các ứng dụng và hiệu trưởng dịch vụ bằng cách đọc các [ứng dụng và đối tượng chính của dịch vụ trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Cách: dùng cổng thông tin để tạo một ứng dụng AZURE AD và hiệu trưởng dịch vụ có thể truy nhập tài nguyên](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) hướng dẫn bạn cách tạo một ứng dụng Azure Active Directory (Azure AD) và hiệu trưởng dịch vụ có thể được sử dụng với điều khiển truy nhập dựa trên vai trò.
4. Với [API chính của dịch vụ](https://docs.microsoft.com/graph/api/resources/serviceprincipal), bạn có thể lập trình quản lý các phiên bản của ứng dụng và điều khiển ứng dụng nào có thể thực hiện trong đối tượng thuê của bạn.
5. [kiểu tài nguyên chính của serviceliệt](https://docs.microsoft.com/graph/api/resources/serviceprincipal) kê tất cả các thuộc tính và phương pháp cho loại tài nguyên hữu ích.
6. [Sự khác biệt về kiểu tài nguyên giữa AZURE AD graph và Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) nổi bật sự khác biệt giữa Azure AD graph và tài nguyên đồ họa Microsoft. Nó hiển thị các tài nguyên có các tên khác nhau hoặc không sẵn dùng; nó cũng có các tài nguyên nổi bật trong phiên bản beta của Microsoft graph nhưng không có trong phiên bản v 1.0.

**Các vấn đề với người dùng khách**

- [Bắt đầu nhanh: thêm người dùng khách vào danh bạ của bạn trong cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) cho bạn biết cách thêm người dùng khách mới vào thư mục Azure AD của bạn qua cổng Azure, gửi lời mời và xem quy trình trả lời thư mời của người dùng khách trông như thế nào.
- [Hướng dẫn: tạo dòng người dùng trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) cho bạn biết cách tạo một số dòng người dùng được đề xuất bằng cách sử dụng cổng thông tin Azure. Nếu bạn đang tìm kiếm thông tin về cách thiết lập dòng chứng danh mật khẩu của chủ sở hữu tài nguyên (ROPC) trong ứng dụng của mình, hãy xem mục đặt cấu hình dòng thông tin xác thực của chủ sở hữu tài nguyên trong Azure AD B2C.
