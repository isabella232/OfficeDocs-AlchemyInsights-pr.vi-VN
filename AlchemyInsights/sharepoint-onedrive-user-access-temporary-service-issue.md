---
title: Sự cố về hiệu suất SharePoint hoặc sự OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093872"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint phát hành OneDrive bị Chậm, Không thể truy nhập hoặc Không sẵn dùng đối với Nhiều Người dùng

Nếu một OneDrive hoặc SharePoint sẵn dùng cho nhiều người dùng trước đây đã có quyền truy nhập, có thể đã xảy ra sự cố dịch vụ tạm thời. [Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).

**Thêm và cấp phép cho người dùng**

Đảm bảo rằng bạn [Gán giấy phép cho người dùng trong Microsoft 365 dành cho doanh nghiệp.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Gán Quyền**

Nếu người dùng đã được gán giấy phép Sharepoint và vẫn nhận được thông báo từ chối quyền truy nhập, vui lòng đảm bảo họ được gán mức [cấp phép thích](https://docs.microsoft.com/sharepoint/understanding-permission-levels) hợp.

**Cân nhắc việc sử dụng tính năng yêu cầu truy nhập**

Tính [năng yêu cầu truy nhập](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép mọi người có thể yêu cầu quyền truy nhập vào nội dung mà hiện thời họ không có quyền xem.

**Allow custom script may cause access denied issues**

There are certain scenarios where the *Allow custom script* feature may be presenting an access denied. Để biết danh sách các tính năng bị ảnh hưởng, những điều cần cân nhắc về bảo mật và khả năng tắt tính năng này. Vui lòng truy cập [vào Cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

