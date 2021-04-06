---
title: Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596042"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo

Windows Virtual Desktop (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất. Công cụ này ghi lại thông tin liên quan đến chẩn đoán mọi khi WVD được người đã gán vai trò WVD. Mỗi Nhật ký có chứa thông tin về vai trò WVD tham gia vào hoạt động này, các thông báo lỗi xuất hiện trong phiên làm việc và thông tin về đối tượng thuê và người dùng. Phân tích Nhật ký Azure có thể được cấu hình để chụp Nhật ký hoạt động được tạo bởi công cụ chẩn đoán bằng cách làm theo các bước sau đây:

1. Tạo không gian làm việc phân tích Nhật ký với [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Kết nối máy tính Windows với Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Lấy ID không gian làm việc và khóa chính của không gian làm việc của bạn. Trình hướng dẫn thiết lập cần thông tin này để cấu hình đúng cho tác nhân và để đảm bảo nó có thể liên lạc với Azure theo dõi.

1. [Đẩy chẩn đoán dữ liệu đến không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284). Bạn có thể đẩy chẩn đoán dữ liệu từ đối tượng thuê WVD của mình vào phân tích Nhật ký cho không gian làm việc của bạn.

1. [Xác định và chẩn đoán](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) các sự cố nằm bên trong hoặc bên ngoài liên quan đến wvd.

Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem dùng phân tích Nhật ký cho tính năng chẩn đoán.