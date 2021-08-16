---
title: Kiểm kê Thiết bị Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014094"
---
# <a name="intune-device-inventory"></a>Kiểm kê Thiết bị Intune

Lưỡi Thiết bị cung cấp thông tin chuyên sâu về người quản trị vào các thiết bị dưới quyền quản lý ở Intune trên cơ sở từng thiết bị. Thông tin hiển thị bao gồm: Phần cứng, ứng dụng được phát hiện, trạng thái Tuân thủ Thiết bị và Trạng thái Cấu hình Thiết bị.

Dữ liệu kiểm kê cho phần cứng và các ứng dụng được phát hiện được thu thập trong một chu kỳ bảy ngày. Các ứng dụng và thành phần cụ thể của phần cứng được báo cáo khác nhau tùy thuộc vào hệ điều hành thiết bị và liệu thiết bị thuộc sở hữu cá nhân hay thuộc sở hữu của công ty.

Để biết thêm thông tin, hãy [xem mục Xem chi tiết thiết bị trong Intune](https://docs.microsoft.com/intune/device-inventory).

**Câu hỏi thường gặp**

Hỏi: Tôi không nhận được danh sách kiểm kê đầy đủ các ứng dụng có trên thiết bị đã đăng ký Intune và Windows bạn. Tại sao không?

Hỏi: Tại thời điểm này, chỉ các ứng dụng hiện đại được liệt kê Windows 10 PC được xác định là thiết bị của công ty. Intune không thu thập thông tin về các ứng dụng Win32 đã cài đặt trên những thiết bị này.

Hỏi: Tại sao số điện thoại không được thu thập từ tất cả các thiết bị?

A: Điện thoại được phân loại là thiết bị công ty trong Intune sẽ không được xác định với số điện thoại đầy đủ của chúng khi bạn chạy báo cáo kiểm kê thiết bị di động chẳng hạn. Số điện thoại trên thiết bị riêng của bạn luôn được che một phần bằng dấu sao (****) và chỉ hiển thị bốn chữ số cuối.