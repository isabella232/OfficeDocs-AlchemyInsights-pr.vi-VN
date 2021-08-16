---
title: Xác định Windows cố trên Màn hình nền Ảo
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
ms.openlocfilehash: 398496448089d4480119a2eb21221dc11f13c6c1f3bcbd931d6c18033f2e734e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987591"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Xác định Windows cố trên Màn hình nền Ảo

Windows Chẩn đoán Máy tính Ảo chỉ sử dụng một lệnh ghép ngắn PowerShell nhưng chứa nhiều tham số tùy chọn để giúp thu hẹp và cách ly các sự cố. Để bắt đầu: 

1. Tải xuống và nhập mô-Windows PowerShell trên Máy tính Ảo. Để biết chi tiết, [hãy xem Windows lệnh ghép ngắn Virtual Desktop để Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Chạy lệnh ghép ngắn sau đây để đăng nhập vào tài khoản của bạn:
    
    Ví dụ: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**LƯU Ý:** Tất cả các truy vấn sử dụng PowerShell phải bao gồm các tham số -UserName hoặc -ActivityID. Để biết các chức năng theo dõi, hãy [xem Dùng Phân tích Nhật ký cho tính năng chẩn đoán.](https://go.microsoft.com/fwlink/?linkid=2126847)

Để lọc các hoạt động chẩn đoán theo người dùng, hãy chạy lệnh ghép ngắn sau đây:

Ví dụ: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Có một danh sách các bộ lọc bạn có thể chạy để chẩn đoán các vấn đề. Để tìm hiểu thêm về chẩn đoán sự cố, hãy xem [Xác định và chẩn đoán Windows cố Màn hình nền Ảo.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Để tìm hiểu thêm về các lỗi thường gặp, hãy [xem mục Lỗi thường gặp trong senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
