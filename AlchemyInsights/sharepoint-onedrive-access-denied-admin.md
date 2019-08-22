---
title: Khắc phục sự cố truy cập từ chối các thư
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503570"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Khắc phục sự cố truy cập từ chối các thư trong Trung tâm quản trị Sharepoint/OneDrive

Nếu bạn nhận được quyền truy cập bị từ chối thư khi cố gắng để duyệt đến một trung tâm quản trị Sharepoint/OneDrive, hãy chắc chắn rằng bạn [gán một giấy phép cho người dùng](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Nếu người dùng có một giấy phép, bạn cũng nên chắc chắn họ là [được gán vai trò người quản trị](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) mà có thể truy cập Trung tâm quản trị.

Vấn đề này cũng có thể xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN). Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau. Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác. Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.

Để giải quyết vấn đề này, bạn nên khôi phục lại UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Lưu ý: Nếu một trung tâm OneDrive hoặc SharePoint Admin là không có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ.  [Kiểm tra bảng điều khiển dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).


