---
title: Yammer cấp phép
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989757"
---
# <a name="yammer-licensing-issues"></a>Yammer cấp phép

Tất cả người dùng phải có giấy phép để sử dụng dịch vụ Yammer Enterprise, nhưng theo mặc định Yammer không yêu cầu người dùng phải có giấy phép để truy nhập vào dịch vụ. Khi người quản trị thay đổi thiết đặt để chặn người dùng Microsoft 365 không có giấy phép Yammer, người dùng không được gán giấy phép Yammer Enterprise sẽ không thể truy nhập vào dịch vụ Yammer của họ. Để biết thêm thông tin, [hãy xem mục Quản lý Yammer phép người dùng trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Khi giấy phép bị loại bỏ khỏi người dùng, ô xếp Yammer hiển thị và các dịch vụ khác có thể sử dụng loại bỏ giấy phép để ẩn các tính năng. Trong các trường hợp khác, các tính năng vẫn có thể xuất hiện nhưng yêu cầu gán giấy phép để hoạt động.  

**Giấy phép không được cập nhật cho người dùng**  

Đôi khi, người dùng được gán giấy phép nhưng vẫn không thể truy nhập vào Yammer. Khả năng cao hơn là xảy ra sự chậm trễ khi quá trình gán giấy phép hàng loạt đang diễn ra. Yammer người dùng có thể không được cập nhật theo cùng một thứ tự với giấy phép được thay đổi trong Azure AD vì hệ thống chạy không đồng bộ. Hãy chờ 24 giờ trước khi mở một trường hợp hỗ trợ để báo cáo sự cố đồng bộ giấy phép.  

**Gán giấy phép hàng loạt**  

Giấy phép có thể được gán thông qua trung tâm quản trị hoặc script PowerShell. Để biết thêm thông tin, [xem mục Gán giấy phép cho](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) người dùng và Gán giấy phép cho tài khoản người dùng Office 365 [PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Bộ trợ giúp của Microsoft không cung cấp hỗ trợ về việc tạo tập lệnh, nhưng có sẵn tài liệu Yammer vụ chuyển nhượng giấy phép mới. Để biết thêm thông tin, [hãy xem Quản lý Yammer phép bằng cách sử dụng Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)