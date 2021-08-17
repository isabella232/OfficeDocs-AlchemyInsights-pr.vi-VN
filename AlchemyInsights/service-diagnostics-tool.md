---
title: Công cụ chẩn đoán dịch vụ dành Windows Bàn làm việc Ảo
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
ms.openlocfilehash: e6c20af2c3fc54b203f3bda5c0c0f00faacd92800566bd507867c4e9fe4a23f1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052336"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Công cụ chẩn đoán dịch vụ dành Windows Bàn làm việc Ảo

Windows Màn hình nền Ảo (WVD) cung cấp một công cụ chẩn đoán cho phép người quản trị xác định lỗi thông qua một giao diện duy nhất. Công cụ này ghi nhật ký thông tin liên quan đến chẩn đoán mỗi khi có người gán vai trò WVD sử dụng WVD. Mỗi nhật ký đều chứa thông tin về vai trò WVD liên quan đến hoạt động, thông báo lỗi xuất hiện trong phiên và thông tin về đối tượng thuê và người dùng. Có thể đặt cấu hình Phân tích Nhật ký Azure để ghi lại nhật ký hoạt động được tạo bởi công cụ chẩn đoán bằng cách làm theo các bước sau:

1. Tạo không gian làm việc Phân tích Nhật ký [với cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129500) hoặc Azure [PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Kết nối Windows tính của bạn sang Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Nhận ID Không gian làm việc và Khóa Chính cho không gian làm việc của bạn. Trình hướng dẫn thiết lập cần thông tin này để đặt cấu hình đúng cách tác nhân và đảm bảo tác nhân đó có thể liên lạc với Azure Monitor.

1. [Đẩy dữ liệu chẩn đoán vào không gian làm việc của bạn](https://go.microsoft.com/fwlink/?linkid=2128284). Bạn có thể đẩy dữ liệu chẩn đoán từ đối tượng thuê WVD sang Phân tích Nhật ký cho không gian làm việc của bạn.

1. [Xác định và chẩn](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) đoán các sự cố nội bộ hoặc bên ngoài liên quan đến WVD.

Để tìm hiểu thêm về việc cấu hình công cụ chẩn đoán dịch vụ cho WVD, hãy xem Dùng Phân tích Nhật ký cho tính năng chẩn đoán.