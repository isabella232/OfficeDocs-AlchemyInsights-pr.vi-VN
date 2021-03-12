---
title: Khắc phục sự cố truy nhập thư bị từ chối
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707976"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Khắc phục sự cố truy nhập bị từ chối thư trong Trung tâm quản trị SharePoint/OneDrive

Nếu bạn nhận được một truy nhập bị từ chối thư khi tìm cách duyệt đến Trung tâm quản trị SharePoint/OneDrive, hãy đảm bảo rằng bạn [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Nếu người dùng có giấy phép, bạn cũng nên đảm bảo rằng chúng được [gán vai trò người quản trị](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) có thể truy nhập vào Trung tâm quản trị.

Sự cố này cũng có thể xảy ra khi người dùng bị xóa bỏ và được tạo lại với cùng tên chính của người dùng (UPN). Tài khoản mới được tạo bằng một giá trị PUID khác (ID duy nhất của Passport). Khi người dùng cố gắng truy nhập vào một tuyển tập trang hoặc OneDrive của họ, người dùng có một con dấu PUID không chính xác. Kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU). Nếu người dùng đã đăng nhập vào SharePoint, sau đó được di chuyển đến OU và resynced khác với SharePoint, họ có thể gặp phải vấn đề này.

Để giải quyết sự cố này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Lưu ý: nếu Trung tâm quản trị OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, thì có thể có sự cố dịch vụ tạm thời.  [Kiểm tra bảng điều khiển trạng thái dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).


