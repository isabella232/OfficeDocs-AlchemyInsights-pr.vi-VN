---
title: Vấn đề hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511170"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không khả dụng cho nhiều người dùng

Nếu một trang web OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời. [Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).

**Thêm và giấy phép người dùng**

Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Microsoft 365 cho doanh nghiệp](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Gán quyền**

Nếu người dùng đã được gán một giấy phép SharePoint và vẫn nhận được thông báo từ chối truy cập, hãy đảm bảo rằng họ có [cấp quyền thích hợp](https://docs.microsoft.com/sharepoint/understanding-permission-levels) chỉ định.

**Xem xét sử dụng tính năng yêu cầu truy cập**

[Tính năng yêu cầu truy cập](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép người khác yêu cầu quyền truy cập vào nội dung mà họ hiện không có quyền xem.

**Cho phép tập lệnh tùy chỉnh có thể gây ra sự cố truy nhập bị từ chối**

Có một số trường hợp nơi *cho phép tính năng kịch bản tuỳ chỉnh* có thể trình bày truy cập bị từ chối. Để có danh sách các tính năng bị ảnh hưởng, cân nhắc bảo mật và khả năng vô hiệu hóa tính năng. Vui lòng truy cập [cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

