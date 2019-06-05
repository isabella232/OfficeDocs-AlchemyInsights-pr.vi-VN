---
title: Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive
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
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715233"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Vấn đề này thường xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau. Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Để giải quyết vấn đề này, bạn nên khôi phục lại UPN ban đầu với các bước trong bài viết, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">khôi phục người dùng trong Office 365.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Sau khi điều này được thực hiện, bạn có thể xác thực người dùng có quyền quản trị trang web OneDrive bằng cách làm theo các bước để <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">thêm của admin cho một người sử dụng OneDrive.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Để biết thêm chi tiết về mức độ cho phép, xem bài viết, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">sự hiểu biết các cấp phép SharePoint.</a>&nbsp;</span></p>
