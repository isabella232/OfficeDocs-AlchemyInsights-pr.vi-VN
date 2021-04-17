---
title: Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824457"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Không thể truy nhập vào Trung tâm quản trị SharePoint hoặc OneDrive

- Nếu site SharePoint hoặc trung tâm quản trị OneDrive của bạn không thể truy nhập được hoặc không sẵn dùng, thì có thể có sự cố dịch vụ tạm thời mà người dùng gặp phải sự chậm trễ hoặc dẫn hướng lỗi khi truy nhập site SharePoint hoặc nội dung OneDrive. Kiểm tra [bảng điều khiển trạng thái dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.

- Người quản trị toàn cầu và SharePoint cần được gán giấy phép SharePoint. Các tài khoản mới được tạo chỉ được gán với một giấy phép SharePoint hoặc vai trò quản trị có thể gặp sự cố khi truy nhập SharePoint, chẳng hạn như "Access bị từ chối" hoặc "không tìm thấy người dùng". Xin vui lòng cung cấp ít nhất 24 giờ để đồng bộ để hoàn tất qua các hệ thống của chúng tôi. Chúng tôi hiểu rằng 24 giờ có thể có vẻ như một thời gian dài. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.

- Người dùng quản lý danh tính đặc quyền ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) có thể nhận được truy nhập bị từ chối nếu có phép cửa sổ thời gian truy nhập là rất nhỏ, hãy xem  [Access bị từ chối đến tài khoản PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).