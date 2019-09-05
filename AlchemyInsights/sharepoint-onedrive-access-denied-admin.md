---
title: Khắc phục sự cố truy cập từ chối thư
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751298"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Khắc phục sự cố truy cập từ chối thư trong SharePoint/OneDrive quản trị Trung tâm

Nếu bạn nhận được thông báo từ chối truy cập khi cố gắng duyệt tới Trung tâm quản trị SharePoint/OneDrive, hãy đảm bảo rằng bạn [gán giấy phép cho người dùng](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Nếu người dùng có giấy phép, bạn cũng nên chắc chắn rằng họ được [gán một vai trò người quản trị](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) có thể truy cập các trung tâm quản trị.

Vấn đề này cũng có thể xảy ra khi người dùng bị xoá và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng giá trị PUID (Passport Unique ID) khác nhau. Khi người dùng cố gắng truy cập vào bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Trường hợp thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một đơn vị tổ chức khác và resynced với SharePoint, họ có thể gặp phải sự cố này.

Để giải quyết vấn đề này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Lưu ý: nếu một trung tâm quản trị OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng trước đây đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.  [Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).


