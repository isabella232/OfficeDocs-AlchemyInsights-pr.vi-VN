---
title: Công cụ chẩn đoán dịch vụ dành Windows Bàn làm việc Ảo
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052408"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Công cụ chẩn đoán dịch vụ dành Windows Bàn làm việc Ảo

Windows Màn hình nền Ảo (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất. Công cụ này ghi nhật ký thông tin liên quan đến chẩn đoán mỗi khi có người gán vai trò WVD sử dụng WVD. Mỗi nhật ký đều chứa thông tin về vai trò WVD liên quan đến hoạt động, thông báo lỗi xuất hiện trong phiên và thông tin về đối tượng thuê và người dùng. Có thể đặt cấu hình Phân tích Nhật ký Azure để ghi lại nhật ký hoạt động được tạo bởi công cụ chẩn đoán. Dưới đây là cách thực hiện:

1. Tạo không gian làm việc Phân tích Nhật ký [với cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc Azure [PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Kết nối Windows tính của bạn sang Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Nhận ID Không gian làm việc và Khóa Chính cho không gian làm việc của bạn. Trình hướng dẫn thiết lập cần thông tin này để đặt cấu hình đúng cách tác nhân và đảm bảo tác nhân đó có thể liên lạc với Azure Monitor.
1. [Đẩy dữ liệu chẩn đoán vào không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284). Bạn có thể đẩy dữ liệu chẩn đoán từ đối tượng thuê WVD sang Phân tích Nhật ký cho không gian làm việc của bạn.
1. [Xác định và chẩn đoán các](https://go.microsoft.com/fwlink/?linkid=2128338) sự cố nội bộ hoặc bên ngoài liên quan đến WVD.

Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem Dùng Phân tích [Nhật ký cho tính năng chẩn đoán.](https://go.microsoft.com/fwlink/?linkid=2128084)
