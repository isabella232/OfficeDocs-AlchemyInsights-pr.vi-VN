---
title: Triển khai phần bổ trợ cho mọi Ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031428"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Triển khai phần bổ trợ cho mọi Ứng dụng Microsoft 365

Triển khai tập trung là cách được đề xuất để triển khai Office bổ trợ cho người dùng và nhóm trong tổ chức của bạn. Để triển khai các phần bổ trợ, hãy làm theo các bước dưới đây:

**Lưu ý:** Để cài đặt các phần bổ trợ dành cho Office người dùng cá nhân, hãy xem mục Xem, quản lý và cài đặt phần bổ trợ [trong Office trình.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Ngoài ra, hãy đảm bảo đã bật tính năng mua riêng Office Store của Store. Để biết chi tiết, hãy xem Ngăn tải xuống phần bổ trợ bằng cách tắt Office Store trên tất cả các máy khách [(Ngoại trừ Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Đảm bảo rằng môi trường của bạn đáp ứng các yêu cầu về triển khai phần bổ trợ sử dụng Triển khai Tập trung. Để biết chi tiết, hãy xem [Yêu cầu](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Đi **tới** Cài đặt  >  **Tích hợp**  >  **Tải ứng** dụng trong trung Trung tâm quản trị Microsoft 365 để triển khai các phần bổ trợ. 

Lưu ý: 

- Ứng dụng Tích hợp yêu cầu người quản trị phải có quyền Quản trị Toàn cầu Exchange quản trị.

- Khi triển khai các phần bổ trợ cho nhiều người dùng, chúng tôi khuyên bạn nên thực hiện gán bằng cách sử dụng các nhóm thay vì người dùng riêng lẻ. Để biết chi tiết, [hãy xem mục Những điều cần cân nhắc khi gán phần bổ trợ cho người dùng và nhóm.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Triển khai Tập trung không hỗ trợ người dùng trong các nhóm lồng hoặc các nhóm có nhóm cha mẹ. Để biết chi tiết, [hãy xem mục Gán người dùng và nhóm.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Đảm bảo rằng Dịch vụ Quản lý Ứng dụng Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') được kích hoạt để người dùng đăng nhập. Để biết chi tiết, hãy xem [Cấu hình thuộc tính ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Nếu bạn gặp sự cố khi triển khai phần bổ trợ bằng Cách sử dụng Ứng dụng Tích hợp, hãy thử triển khai bằng [Cách sử dụng Phần Bổ trợ.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Để biết thêm thông tin, hãy xem:

[Triển khai các phần bổ trợ trong trung tâm quản trị](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Quản lý phần bổ trợ trong trung tâm quản trị](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Sử dụng các lệnh ghép ngắn PowerShell Triển khai Tập trung để quản lý phần bổ trợ](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Phát hành Office bổ trợ bằng Triển khai Tập trung thông qua Trung tâm quản trị Microsoft 365](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Khắc phục sự cố: Người dùng không nhìn thấy các phần bổ trợ](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Khắc phục lỗi người dùng Office Bổ trợ](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)