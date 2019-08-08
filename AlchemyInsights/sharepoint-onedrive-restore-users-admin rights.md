---
title: Khắc phục sự cố truy cập từ chối các thư đến OneDrive cho các trang web kinh doanh
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232576"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Khắc phục sự cố truy cập từ chối các thư đến OneDrive cho các trang web kinh doanh

Vấn đề này thường xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau. Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.

1. Để giải quyết vấn đề này, bạn nên khôi phục lại các UPN ban đầu với các bước trong bài viết,[khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Nếu bạn không thể khôi phục người dùng ban đầu bạn nên loại bỏ người dùng cũ khỏi OneDrive trang web bằng cách sử dụng các bước này, [loại bỏ người dùng khỏi danh sách thông tin người dùng](). 
3. Sau khi điều này được thực hiện, bạn có thể xác thực người dùng có quyền quản trị trang web OneDrive bằng cách làm theo các bước để [Thêm admin của cho một người sử dụng OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Để biết thêm chi tiết về mức độ cho phép, hãy xem bài viết, [sự hiểu biết cho phép cấp trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
