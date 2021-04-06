---
title: Xác định các sự cố của Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596039"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Xác định các sự cố của Windows Virtual Desktop

Windows Virtual Desktop Diagnostics chỉ sử dụng một lệnh ghép ngắn PowerShell nhưng chứa nhiều tham số tùy chọn để giúp thu hẹp và cô lập các vấn đề. Để bắt đầu: 

1. Tải xuống và nhập mô-đun Windows Virtual Desktop PowerShell. Để biết chi tiết, hãy xem các [lệnh ghép ngắn trên máy tính chạy Windows ảo cho Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Chạy lệnh ghép ngắn sau đây để đăng nhập vào tài khoản của bạn:
    
    Mẫu `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**Lưu ý:** Tất cả các truy vấn bằng PowerShell phải bao gồm các tham số-tên người dùng hoặc-ActivityID. Để biết các chức năng giám sát, hãy xem dùng [phân tích Nhật ký cho tính năng chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2126847).

Để lọc các hoạt động chẩn đoán theo người dùng, hãy chạy lệnh ghép ngắn sau đây:

Mẫu `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Có một danh sách các bộ lọc mà bạn có thể chạy để chẩn đoán vấn đề. Để tìm hiểu thêm về các vấn đề về chẩn đoán, hãy xem [xác định và chẩn đoán sự cố của Windows Virtual trên máy tính bàn](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Để tìm hiểu thêm về các lỗi phổ biến, hãy xem các [lỗi thường gặp trong senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
