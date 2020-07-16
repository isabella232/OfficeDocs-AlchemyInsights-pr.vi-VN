---
title: Vấn đề cấp phép yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148430"
---
# <a name="yammer-licensing-issues"></a>Vấn đề cấp phép yammer

Tất cả người dùng phải có giấy phép sử dụng dịch vụ yammer Enterprise, nhưng theo mặc định yammer không yêu cầu người dùng có giấy phép truy cập Dịch vụ. Khi quản trị viên thay đổi thiết đặt chặn Microsoft 365 người dùng không có giấy phép yammer, người dùng không được gán giấy phép yammer Enterprise không thể truy cập Dịch vụ yammer. Để biết thêm thông tin, xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Khi giấy phép được loại bỏ khỏi người dùng, ngăn xếp yammer không còn được hiển thị và các dịch vụ khác có thể sử dụng loại bỏ giấy phép để ẩn các tính năng. Trong các trường hợp khác, các tính năng vẫn có thể xuất hiện nhưng yêu cầu gán giấy phép hoạt động.  

**Giấy phép không được Cập Nhật cho người dùng**  

Đôi khi, người dùng được gán giấy phép nhưng vẫn không thể truy cập yammer. Sự chậm trễ có nhiều khả năng xảy ra khi gán giấy phép hàng loạt đang tiến triển. Yammer người dùng có thể không được Cập Nhật theo thứ tự như giấy phép được thay đổi trong Azure AD vì hệ thống chạy không đồng bộ. Đợi tối đa 24 giờ trước khi mở một trường hợp hỗ trợ để báo cáo sự cố đồng bộ hoá giấy phép.  

**Gán giấy phép số lượng lớn**  

Giấy phép có thể được chỉ định thông qua Trung tâm quản trị hoặc script PowerShell. Để biết thêm thông tin, xem [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) và [gán giấy phép cho tài khoản người dùng với Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Hỗ trợ của Microsoft không cung cấp hỗ trợ tạo tập lệnh, nhưng tài liệu về yammer cấp phép gán có sẵn. Để biết thêm thông tin, xem [quản lý giấy phép yammer bằng cách sử dụng Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).