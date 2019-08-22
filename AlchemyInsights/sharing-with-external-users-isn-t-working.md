---
title: Chia sẻ với người dùng bên ngoài không hoạt động
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502253"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Sửa chữa các vấn đề về chia sẻ nội dung SharePoint với người dùng bên ngoài

Đảm bảo rằng bên ngoài chia sẻ được bật cho tổ chức của bạn:
  
1. Đi đến các [dịch vụ &amp; add-in trang trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), và nhấp vào **các trang web**.
    
2. Đảm bảo rằng các thiết lập được bật "On." Nếu "Chỉ người dùng bên ngoài hiện tại" được chọn, hãy chắc chắn rằng người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.
    
Đảm bảo rằng ngoài việc chia sẻ nó bật lên cho trang web. Đối với một bộ sưu tập cổ điển trang web:
  
1. Trong Trung tâm quản trị mới SharePoint, trong ngăn bên trái, nhấp vào **các trang web**.
    
2. Chọn các trang web hoặc các trang web và trên các ribbon, hãy nhấp vào **chia sẻ**.
    
Cho một trang web đội thuộc về một nhóm Office 365, hoặc một trang web thông tin liên lạc:
  
- Các loại trang web mới có chia sẻ cùng cài đặt như thiết lập trên toàn tổ chức của bạn, trừ khi thiết lập phạm vi tổ chức cho phép chia sẻ tập tin bằng cách sử dụng liên kết mà không cần đăng nhập. Trong trường hợp này, các trang web cho phép chia sẻ với các mới và hiện tại bên ngoài người dùng đăng nhập. Để thay đổi các thiết lập cho trang web cụ thể, sử dụng trung tâm quản trị SharePoint mới hoặc PowerShell. [Tìm hiểu thêm](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Cài đặt chia sẻ bên ngoài cho bất kỳ trang web có thể hạn chế hơn so với các thiết lập toàn tổ chức của bạn, nhưng không nhiều hơn permissive hơn thiết đặt phạm vi tổ chức. 
  

