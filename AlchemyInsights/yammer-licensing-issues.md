---
title: Các vấn đề về cấp phép yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657298"
---
# <a name="yammer-licensing-issues"></a>Các vấn đề về cấp phép yammer

Tất cả người dùng phải có giấy phép sử dụng dịch vụ yammer Enterprise nhưng theo mặc định là yammer không yêu cầu người dùng có giấy phép truy nhập vào dịch vụ. Khi người quản trị thay đổi thiết đặt để chặn người dùng Microsoft 365 không có giấy phép yammer, người dùng không gán giấy phép yammer Enterprise không thể truy nhập vào dịch vụ yammer. Để biết thêm thông tin, hãy xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Khi giấy phép được loại bỏ khỏi người dùng, lát xếp yammer không còn được hiển thị và các dịch vụ khác có thể sử dụng loại bỏ giấy phép để ẩn các tính năng. Trong các trường hợp khác, các tính năng vẫn có thể xuất hiện nhưng yêu cầu gán giấy phép để hoạt động.  

**Giấy phép không nhận được Cập Nhật cho người dùng**  

Đôi khi, người dùng được gán giấy phép nhưng vẫn không thể truy nhập vào yammer. Sự chậm trễ có nhiều khả năng xảy ra khi việc gán giấy phép hàng loạt đang được tiến hành. Người dùng yammer có thể không được Cập Nhật theo cùng một thứ tự như giấy phép được thay đổi trong Azure AD vì hệ thống chạy asynchronously. Chờ tối đa 24 giờ trước khi mở một trường hợp hỗ trợ để báo cáo các vấn đề về đồng bộ cấp phép.  

**Gán hàng loạt giấy phép**  

Có thể gán giấy phép thông qua Trung tâm quản trị hoặc script PowerShell. Để biết thêm thông tin, hãy xem mục [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) và [gán giấy phép cho tài khoản người dùng với Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Hỗ trợ của Microsoft không cung cấp trợ giúp với việc tạo script nhưng tài liệu hướng dẫn giấy phép yammer sẵn dùng. Để biết thêm thông tin, hãy xem [quản lý giấy phép yammer bằng cách dùng Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).