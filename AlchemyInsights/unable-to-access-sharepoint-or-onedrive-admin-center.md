---
title: Không thể truy cập vào Trung tâm quản trị SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716477"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Không thể truy cập vào Trung tâm quản trị SharePoint hoặc OneDrive

- Nếu trang web trung tâm quản trị SharePoint hoặc OneDrive của bạn không truy nhập được hoặc không khả dụng, có thể có sự cố dịch vụ tạm thời trong đó người dùng gặp phải các lỗi điều hướng hoặc chậm trễ liên tục khi truy cập các trang web SharePoint hoặc nội dung OneDrive. Kiểm tra [bảng điều khiển tình trạng dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.

- Toàn cầu và SharePoint quản trị viên cần phải được gán một giấy phép SharePoint. Tài khoản mới được tạo chỉ được gán với giấy phép SharePoint hoặc vai trò quản trị có thể gặp phải sự cố truy cập SharePoint, như "truy cập bị từ chối" hoặc "người dùng không tìm thấy." Xin vui lòng cho ít nhất 24 giờ để đồng bộ để hoàn thành trên toàn hệ thống của chúng tôi. Chúng tôi hiểu rằng 24 giờ có thể có vẻ như một thời gian dài. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.

- Người dùng đặc quyền Identity quản lý ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) có thể nhận được truy cập bị từ chối nếu cho phép truy cập thời gian cửa sổ là rất nhỏ, xem [truy cập từ chối tài khoản PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).