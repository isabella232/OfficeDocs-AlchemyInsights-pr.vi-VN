---
title: Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749500"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive

- Nếu site SharePoint hoặc trung tâm quản trị OneDrive của bạn không thể truy nhập được hoặc không sẵn dùng, thì có thể có sự cố dịch vụ tạm thời mà người dùng gặp phải sự chậm trễ hoặc dẫn hướng lỗi khi truy nhập site SharePoint hoặc nội dung OneDrive. Kiểm tra [bảng điều khiển trạng thái dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.

- Người quản trị toàn cầu và SharePoint cần được gán giấy phép SharePoint. Các tài khoản mới được tạo chỉ được gán với một giấy phép SharePoint hoặc vai trò quản trị có thể gặp sự cố khi truy nhập SharePoint, chẳng hạn như "Access bị từ chối" hoặc "không tìm thấy người dùng". Xin vui lòng cung cấp ít nhất 24 giờ để đồng bộ để hoàn tất qua các hệ thống của chúng tôi. Chúng tôi hiểu rằng 24 giờ có thể có vẻ như một thời gian dài. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.

- Người dùng quản lý danh tính đặc quyền ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) có thể nhận được truy nhập bị từ chối nếu có phép cửa sổ thời gian truy nhập là rất nhỏ, hãy xem  [Access bị từ chối đến tài khoản PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).