---
title: Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680237"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Công cụ chẩn đoán dịch vụ cho máy tính để bàn Windows ảo

Windows Virtual Desktop (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất. Công cụ này ghi lại thông tin liên quan đến chẩn đoán mọi khi WVD được người đã gán vai trò WVD. Mỗi Nhật ký có chứa thông tin về vai trò WVD tham gia vào hoạt động này, các thông báo lỗi xuất hiện trong phiên làm việc và thông tin về đối tượng thuê và người dùng. Phân tích Nhật ký Azure có thể được cấu hình để chụp Nhật ký hoạt động được tạo bởi công cụ chẩn đoán. Dưới đây là cách thực hiện:

1. Tạo không gian làm việc phân tích Nhật ký với [cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Kết nối máy tính Windows với Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Lấy ID không gian làm việc và khóa chính của không gian làm việc của bạn. Trình hướng dẫn thiết lập cần thông tin này để cấu hình đúng cho tác nhân và để đảm bảo nó có thể liên lạc với Azure theo dõi.
1. [Đẩy chẩn đoán dữ liệu đến không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284). Bạn có thể đẩy chẩn đoán dữ liệu từ đối tượng thuê WVD của mình vào phân tích Nhật ký cho không gian làm việc của bạn.
1. [Xác định và chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2128338) các sự cố nằm bên trong hoặc bên ngoài liên quan đến wvd.

Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem [dùng phân tích Nhật ký cho tính năng chẩn đoán](https://go.microsoft.com/fwlink/?linkid=2128084).
