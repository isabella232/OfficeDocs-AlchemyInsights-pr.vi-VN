---
title: Không thể truy nhập trung SharePoint hoặc OneDrive trị viên
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
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020466"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Không thể truy nhập trung SharePoint hoặc OneDrive trị viên

- Nếu site Trung tâm quản trị SharePoint hoặc OneDrive của bạn không thể truy nhập hoặc không khả dụng, có thể đã xảy ra sự cố dịch vụ tạm thời trong đó người dùng gặp phải lỗi dẫn hướng hoặc chậm trễ không liên tục khi truy nhập site SharePoint hoặc nội dung OneDrive. Kiểm tra bảng [điều khiển Tình trạng dịch](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vụ để xem liệu tổ chức của bạn có bị ảnh hưởng không.

- Người quản trị toàn SharePoint toàn cầu cần được gán giấy phép SharePoint toàn cầu. Các tài khoản mới được tạo vừa được gán với vai trò Giấy phép hoặc Người quản trị SharePoint có thể gặp sự cố khi truy nhập SharePoint, chẳng hạn như "truy nhập bị từ chối" hoặc "không tìm thấy người dùng". Vui lòng dành ít nhất 24 giờ để quá trình đồng bộ hoàn tất trên các hệ thống của chúng tôi. Chúng tôi hiểu rằng 24 giờ có thể trông giống như một khoảng thời gian dài. Trong nhiều trường hợp, chúng tôi đang nỗ lực tìm giải pháp.

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) người dùng có thể nhận được quyền truy nhập bị từ chối nếu khung thời gian truy nhập được cho phép là rất nhỏ, hãy xem Truy nhập bị từ [chối đối với tài khoản PIM.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)