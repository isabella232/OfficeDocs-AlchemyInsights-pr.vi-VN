---
title: Khắc phục sự cố truy nhập vào thư bị từ chối
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085250"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Khắc phục sự cố truy nhập thông báo Bị từ chối trong Trung tâm Quản OneDrive Sharepoint/OneDrive

If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you assign a [license to the user.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Nếu người dùng có giấy phép, bạn cũng nên đảm bảo họ được gán vai trò [người](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) quản trị có thể truy nhập vào trung tâm quản trị.

Sự cố này cũng có thể xảy ra khi người dùng bị xóa và tạo lại với cùng tên chính người dùng (UPN). Tài khoản mới được tạo bằng cách sử dụng giá trị PUID khác (ID Duy nhất hộ chiếu). When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. Kịch bản thứ hai liên quan đến đồng bộ hóa thư mục với một đơn vị tổ chức (OU) Active Directory. Nếu người dùng đã đăng nhập vào SharePoint, rồi được chuyển sang OU khác và được đồng bộ lại với SharePoint thì họ có thể gặp sự cố này.

Để giải quyết sự cố này, bạn nên khôi phục UPN gốc theo các bước trong bài viết Khôi phục [người dùng trong Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Lưu ý: Nếu một trung OneDrive hoặc SharePoint trị viên không khả dụng cho nhiều người dùng trước đây đã có quyền truy nhập thì có thể xảy ra sự cố dịch vụ tạm thời.  [Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).


