---
title: Tính năng chia sẻ với người dùng bên ngoài không hoạt động
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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910388"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Khắc phục sự cố chia SharePoint nội dung với người dùng bên ngoài

Đảm bảo đã bật chia sẻ với bên ngoài cho tổ chức của bạn:
  
1. Truy nhập trang [Phần bổ trợ dịch vụ trong &amp; Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), rồi bấm vào **Site**.
    
2. Đảm bảo rằng cài đặt được chuyển thành "Bật". Nếu chọn "Chỉ người dùng bên ngoài hiện có", hãy đảm bảo người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.
    
Đảm bảo đã bật chia sẻ với bên ngoài cho site. Đối với tuyển tập site cổ điển:
  
1. Trong trung tâm quản SharePoint mới, ở ngăn bên trái, bấm **vào site.**
    
2. Chọn site hoặc các site và trên dải băng, bấm Chia **sẻ.**
    
Đối với site nhóm thuộc nhóm Microsoft 365 hoặc site liên lạc:
  
- Các loại site mới này có thiết đặt chia sẻ giống như thiết đặt trong toàn tổ chức của bạn, trừ khi thiết đặt trên toàn tổ chức cho phép chia sẻ tệp bằng các nối kết không yêu cầu đăng nhập. Trong trường hợp này, site cho phép chia sẻ với người dùng bên ngoài mới và hiện có đăng nhập. Để thay đổi thiết đặt cho các site cụ thể, hãy sử dụng trung SharePoint quản trị mới hoặc PowerShell. [Tìm hiểu thêm.](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Thiết đặt chia sẻ ra bên ngoài cho bất kỳ site nào có thể hạn chế hơn thiết đặt toàn tổ chức của bạn, nhưng cũng không có quyền hơn thiết đặt trong toàn tổ chức. 
  

