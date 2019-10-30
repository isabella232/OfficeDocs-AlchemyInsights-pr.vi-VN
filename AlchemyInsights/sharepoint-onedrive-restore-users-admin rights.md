---
title: Khắc phục sự cố truy cập từ chối thư vào OneDrive cho doanh nghiệp trang web
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766733"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Khắc phục sự cố truy cập từ chối thư vào OneDrive cho doanh nghiệp trang web

Vấn đề này thường xảy ra khi người dùng bị xoá và tạo lại cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng giá trị PUID (Passport Unique ID) khác nhau. Khi người dùng cố gắng truy cập vào bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Trường hợp thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một đơn vị tổ chức khác và resynced với SharePoint, họ có thể gặp phải sự cố này.

1. Để giải quyết vấn đề này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Nếu bạn không thể khôi phục người dùng ban đầu, bạn nên xoá người dùng cũ khỏi trang web OneDrive bằng cách sử dụng các bước sau, [xoá người dùng khỏi danh sách thông tin người dùng](). 
3. Sau khi hoàn tất, bạn có thể xác minh người dùng có quyền quản trị trang web OneDrive bằng cách làm theo các bước để [Thêm quản trị viên cho onedrive của người dùng](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Để biết thêm thông tin về cấp quyền, hãy xem bài viết, [hiểu cấp quyền trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
