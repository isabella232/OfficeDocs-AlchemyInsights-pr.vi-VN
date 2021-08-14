---
title: Khắc phục sự cố truy nhập vào thư bị từ chối
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957995"
---
# <a name="troubleshoot-access-denied-messages"></a>Khắc phục sự cố truy nhập vào thư bị từ chối

Nếu bạn đang nhận được thông báo từ chối truy nhập khi tìm cách duyệt site Sharepoint Online, vui lòng xem các bài viết dưới đây.

**Thêm và Cấp phép cho người dùng**

Đảm bảo rằng bạn [Gán giấy phép cho người dùng trong Microsoft 365 dành cho doanh nghiệp.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)

**Gán Quyền**

Nếu người dùng đã được gán giấy phép Sharepoint và vẫn nhận được thông báo từ chối quyền truy nhập, vui lòng đảm bảo họ được gán [mức cấp phép thích hợp.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Cân nhắc việc sử dụng tính năng yêu cầu truy nhập**

Tính [năng yêu cầu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) truy nhập cho phép mọi người có thể yêu cầu quyền truy nhập vào nội dung mà hiện thời họ không có quyền xem. 

**Allow custom script may cause access denied issues**

Có một số kịch bản nhất định mà tính năng "Cho phép tập lệnh tùy chỉnh" có thể đang trình bày quyền truy nhập bị từ chối. Để biết danh sách các tính năng bị ảnh hưởng, những điều cần cân nhắc về bảo mật và khả năng tắt tính năng này. Vui lòng truy cập , [Cho phép hoặc ngăn chặn script tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Lưu ý: Nếu một OneDrive hoặc site SharePoint sẵn dùng cho nhiều người dùng trước đây đã có quyền truy nhập, có thể đã xảy ra sự cố dịch vụ tạm thời. [Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).


  

