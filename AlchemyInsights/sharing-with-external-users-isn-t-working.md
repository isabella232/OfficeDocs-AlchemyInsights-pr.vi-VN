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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304391"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Khắc phục sự cố chia SharePoint nội dung với người dùng bên ngoài

Đảm bảo đã bật chia sẻ với bên ngoài cho tổ chức của bạn:
  
1. Truy nhập trang [Phần bổ trợ dịch vụ trong &amp; Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), rồi bấm vào **Site**.
    
2. Đảm bảo rằng cài đặt được chuyển thành "Bật". Nếu chọn "Chỉ người dùng bên ngoài hiện có", hãy đảm bảo người dùng bên ngoài được liệt kê trong danh Trung tâm quản trị Microsoft 365.
    
Đảm bảo đã bật chia sẻ với bên ngoài cho site. Đối với tuyển tập site cổ điển:
  
1. Trong trung tâm quản SharePoint mới, ở ngăn bên trái, bấm **vào site.**
    
2. Chọn site hoặc các site và trên dải băng, hãy bấm Chia **sẻ.**
    
Đối với site nhóm thuộc nhóm Microsoft 365 hoặc site liên lạc:
  
- Các loại site mới này có thiết đặt chia sẻ giống như thiết đặt trong toàn tổ chức của bạn, trừ khi thiết đặt trên toàn tổ chức cho phép chia sẻ tệp bằng các nối kết không yêu cầu đăng nhập. Trong trường hợp này, site cho phép chia sẻ với người dùng bên ngoài mới và hiện có đăng nhập. Để thay đổi thiết đặt cho các site cụ thể, hãy sử dụng trung tâm quản SharePoint hoặc PowerShell mới. [Tìm hiểu thêm.](https://go.microsoft.com/fwlink/?linkid=871863)
    
**Lưu** ý : Thiết đặt chia sẻ với bên ngoài cho site bất kỳ có thể hạn chế hơn thiết đặt toàn tổ chức của bạn, nhưng không có quyền hơn thiết đặt toàn tổ chức. 
  

