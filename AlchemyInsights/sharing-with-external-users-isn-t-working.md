---
title: Chia sẻ với người dùng bên ngoài không hoạt động
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691597"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Khắc phục sự cố chia sẻ nội dung SharePoint với người dùng bên ngoài

Đảm bảo chia sẻ bên ngoài được bật cho tổ chức của bạn:
  
1. Đi đến [trang bổ trợ dịch vụ &amp; trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), rồi bấm vào **site**.
    
2. Đảm bảo cài đặt được bật thành "bật." Nếu "chỉ những người dùng bên ngoài hiện có" được chọn, hãy đảm bảo rằng người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.
    
Đảm bảo chia sẻ bên ngoài nó bật đối với trang. Đối với tuyển tập trang cổ điển:
  
1. Trong Trung tâm quản trị SharePoint mới, trong ngăn bên trái, hãy bấm **site**.
    
2. Chọn trang hoặc site và trên Ribbon, bấm **chia sẻ**.
    
Đối với một site nhóm thuộc nhóm Microsoft 365 hoặc một site liên lạc:
  
- Những loại site mới này có cùng thiết đặt chia sẻ như thiết đặt toàn bộ tổ chức của bạn, trừ khi thiết đặt toàn bộ tổ chức cho phép chia sẻ tệp bằng các liên kết không yêu cầu đăng nhập. Trong trường hợp này, các site cho phép chia sẻ với những người dùng bên ngoài mới và hiện có đăng nhập. Để thay đổi thiết đặt cho các site cụ thể, hãy sử dụng trung tâm quản trị SharePoint mới hoặc PowerShell. [Tìm hiểu thêm](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Thiết đặt chia sẻ bên ngoài cho bất kỳ trang nào có thể được thêm hạn chế so với cài đặt phạm vi tổ chức của bạn, nhưng không được nhiều hơn so với cài đặt phạm vi tổ chức. 
  

