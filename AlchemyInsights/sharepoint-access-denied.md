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
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691705"
---
# <a name="troubleshoot-access-denied-messages"></a>Khắc phục sự cố truy nhập thư bị từ chối

Nếu bạn nhận được một truy nhập bị từ chối thư khi tìm cách duyệt một site SharePoint Online, vui lòng xem các bài viết dưới đây.

**Thêm và cấp giấy phép cho người dùng**

Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Gán quyền**

Nếu người dùng đã được gán giấy phép SharePoint và vẫn nhận được một thông báo bị từ chối truy nhập, vui lòng đảm bảo họ có [cấp độ quyền thích hợp được gán](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Cân nhắc việc sử dụng tính năng yêu cầu truy nhập**

Tính năng [truy nhập yêu cầu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép mọi người yêu cầu quyền truy nhập vào nội dung mà họ hiện không có quyền để xem. 

**Cho phép script tùy chỉnh có thể khiến các vấn đề bị từ chối truy nhập**

Có một số kịch bản nhất định mà tính năng "cho phép tùy chỉnh" có thể đang trình bày một truy nhập bị từ chối. Để biết danh sách các tính năng bị ảnh hưởng, cân nhắc về bảo mật và khả năng vô hiệu hóa tính năng. Vui lòng truy nhập, [cho phép hoặc ngăn chặn Script tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Lưu ý: Nếu site OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, có thể có sự cố dịch vụ tạm thời. [Kiểm tra bảng điều khiển trạng thái dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).


  

