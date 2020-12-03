---
title: Xóa đối tượng thuê
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564875"
---
# <a name="delete-tenant"></a>Xóa đối tượng thuê

Để xóa một Azure AD, hãy đảm bảo:
- Bạn là người quản trị toàn cầu trên thư mục.
- Bạn không đăng nhập bằng tài khoản có thư mục mặc định, chẳng hạn như contoso.onmicrosoft.com trong tài khoản đã đăng nhập, chẳng hạn như admin@contoso.onmicrosoft.com.
- Loại bỏ mọi ứng dụng hiện hoạt trong thư mục trước khi xóa. Để loại bỏ các ứng dụng hiện hoạt, hãy dẫn hướng đến đăng ký ứng dụng và loại bỏ các ứng dụng hiện có.
- Không có đăng ký hiện hoạt nào đối với bất kỳ dịch vụ Microsoft Online nào, chẳng hạn như Microsoft Azure, Office 365 hoặc Azure AD Premium liên kết trên thư mục. Chuyển các đăng ký của bạn hoặc đẩy nhanh việc hủy bỏ các đăng ký hiện hoạt thông qua Azure support và thanh toán. Tìm hiểu thêm về cách hủy bỏ đăng ký Office 365 và Azure. Để được hướng dẫn liên kết hoặc thêm đăng ký hiện có vào một đối tượng thuê, hãy xem [liên kết hoặc thêm đăng ký Azure vào đối tượng thuê AZURE AD của bạn](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Không có giấy phép hiện hoạt. Để loại bỏ giấy phép, hãy xem [làm thế nào để loại bỏ đăng ký để loại bỏ giấy phép](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Không có người dùng hiện hoạt nào khác trong thư mục bên cạnh mình là người quản trị toàn cầu khi cố gắng xóa Azure AD. Loại bỏ bất kỳ người dùng hiện hoạt nào khác và bất kỳ phụ thuộc nào trong tên miền tùy chỉnh trong đối tượng thuê cũng sẽ cần bị loại bỏ, chẳng hạn như người dùng được tạo bằng admin@contoso.com.

Để biết thêm các bước chi tiết về cách thức:
- Xóa bỏ "Azure Active Directory" hoặc "đăng ký", hãy xem [xóa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Loại bỏ các ứng dụng trong thư mục, hãy xem [loại bỏ các ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
