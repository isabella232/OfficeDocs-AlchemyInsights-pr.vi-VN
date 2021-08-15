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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993915"
---
# <a name="delete-tenant"></a>Xóa đối tượng thuê

Để xóa Azure AD, hãy đảm bảo:
- Bạn là Người quản trị Toàn cầu trên thư mục.
- Bạn KHÔNG đăng nhập bằng tài khoản có thư mục mặc định như contoso.onmicrosoft.com trong tài khoản đã đăng nhập, chẳng hạn như admin@contoso.onmicrosoft.com.
- Loại bỏ mọi ứng dụng hiện hoạt trong thư mục trước khi xóa. Để loại bỏ các ứng dụng hiện hoạt, dẫn hướng đến Đăng ký ứng dụng và loại bỏ các ứng dụng hiện có.
- Không có đăng ký hiện hoạt cho mọi Dịch vụ Trực tuyến của Microsoft, chẳng hạn như Microsoft Azure, Office 365 hoặc Azure AD Premium liên kết trên thư mục. Chuyển gói đăng ký của bạn hoặc đẩy nhanh việc hủy bỏ đăng ký hiện hoạt thông qua Hỗ trợ và Thanh toán Azure. Tìm hiểu thêm về Cách Hủy bỏ đăng ký Office 365 Azure và Azure. Để biết hướng dẫn liên kết hoặc thêm đăng ký hiện có cho đối tượng thuê, hãy xem mục Liên kết hoặc thêm đăng ký Azure vào đối [tượng thuê Azure AD của bạn.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Không có giấy phép Hiện hoạt. Để loại bỏ giấy phép, hãy xem [Cách loại bỏ đăng ký để loại bỏ giấy phép](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Ngoài chính bạn, không có người dùng hiện hoạt nào khác trong thư mục với tư cách là Người quản trị Toàn cầu khi tìm cách xóa Azure AD. Loại bỏ mọi người dùng hiện hoạt khác và mọi phụ thuộc vào tên miền riêng trong đối tượng thuê cũng sẽ cần phải được loại bỏ, chẳng hạn như người dùng được tạo bằng tên miền admin@contoso.com.

Để biết thêm các bước chi tiết về cách thực hiện:
- Xóa "Azure Active Directory" hoặc "đăng ký", xem [mục Xóa Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Loại bỏ các ứng dụng trong thư mục, hãy xem [Loại bỏ Ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
