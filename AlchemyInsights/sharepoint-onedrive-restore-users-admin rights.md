---
title: Khắc phục sự cố Access bị từ chối thư vào các site OneDrive for Business
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670638"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Khắc phục sự cố Access bị từ chối thư vào các site OneDrive for Business

Sự cố này thường xảy ra khi người dùng bị xóa bỏ và được tạo lại với cùng tên chính của người dùng (UPN). Tài khoản mới được tạo bằng một giá trị PUID khác (ID duy nhất của Passport). Khi người dùng cố gắng truy nhập vào một tuyển tập trang hoặc OneDrive của họ, người dùng có một con dấu PUID không chính xác. Kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, sau đó được di chuyển đến OU và resynced khác với SharePoint, họ có thể gặp phải vấn đề này.

1. Để giải quyết sự cố này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Nếu bạn không thể khôi phục người dùng ban đầu, bạn nên loại bỏ người dùng cũ khỏi site OneDrive bằng cách sử dụng các bước này, hãy [loại bỏ người dùng khỏi danh sách thông tin người dùng](). 
3. Sau khi hoàn thành xong, bạn có thể xác nhận người dùng có quyền quản trị đối với site OneDrive bằng cách làm theo các bước để [Thêm người quản trị cho OneDrive của người dùng](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Để biết thêm thông tin về các mức cấp phép, hãy xem bài viết, [Tìm hiểu các mức cấp phép trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
