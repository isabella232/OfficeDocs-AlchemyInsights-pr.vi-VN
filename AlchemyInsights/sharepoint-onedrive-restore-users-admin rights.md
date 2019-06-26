---
title: Khắc phục sự cố truy cập từ chối các thư đến OneDrive cho các trang web kinh doanh
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223446"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Khắc phục sự cố truy cập từ chối các thư đến OneDrive cho các trang web kinh doanh

Vấn đề này thường xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau. Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.

Để giải quyết vấn đề này, bạn nên khôi phục lại các UPN ban đầu với các bước trong bài viết,[khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Sau khi điều này được thực hiện, bạn có thể xác thực người dùng có quyền quản trị trang web OneDrive bằng cách làm theo các bước để [Thêm admin của cho một người sử dụng OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Để biết thêm chi tiết về mức độ cho phép, hãy xem bài viết, [sự hiểu biết cho phép cấp trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
