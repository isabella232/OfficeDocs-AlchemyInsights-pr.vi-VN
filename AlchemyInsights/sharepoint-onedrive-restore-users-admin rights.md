---
title: Khắc phục sự cố Truy nhập bị từ chối đối với OneDrive for Business site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957815"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Khắc phục sự cố Truy nhập bị từ chối đối với OneDrive for Business site

Sự cố này thường xảy ra nhất khi người dùng bị xóa và tạo lại với cùng tên chính người dùng (UPN). Tài khoản mới được tạo bằng cách sử dụng giá trị PUID khác (ID Duy nhất hộ chiếu). When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. Kịch bản thứ hai liên quan đến đồng bộ hóa thư mục với một đơn vị tổ chức (OU) Active Directory. Nếu người dùng đã đăng nhập vào SharePoint, rồi được chuyển sang OU khác và được đồng bộ lại với SharePoint thì họ có thể gặp sự cố này.

1. Để giải quyết sự cố này, bạn nên khôi phục UPN gốc theo các bước trong bài viết, Khôi [phục người dùng trong Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list.]() 
3. Sau khi thực hiện xong, bạn có thể xác nhận người dùng có quyền quản trị đối với site OneDrive bằng cách làm theo các bước để Thêm người quản trị cho tài khoản người [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Để biết thêm thông tin về các mức cấp phép, hãy xem bài viết Tìm [hiểu các mức cấp phép SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
