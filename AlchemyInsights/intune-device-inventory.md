---
title: Kho thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440482"
---
# <a name="intune-device-inventory"></a>Kho thiết bị InTune

Thiết bị Blade cung cấp thông tin chi tiết quản trị viên vào thiết bị quản lý trong InTune trên cơ sở mỗi thiết bị. Thông tin hiển thị bao gồm: phần cứng, phát hiện các ứng dụng, trạng thái tuân thủ thiết bị và trạng thái cấu hình thiết bị.

Kiểm kê dữ liệu cho phần cứng và phát hiện các ứng dụng được thu thập trên một chu kỳ bảy ngày. Các ứng dụng và các yếu tố cụ thể của phần cứng báo cáo khác nhau tùy thuộc vào hệ điều hành thiết bị và cho dù thiết bị là cá nhân hoặc công ty sở hữu.

Để biết thêm thông tin, xem [xem chi tiết thiết bị trong InTune](https://docs.microsoft.com/intune/device-inventory).

**Faq**

Câu hỏi: tôi không nhận được danh sách đầy đủ các ứng dụng hiện có trên các thiết bị Windows được đăng ký InTune. Tại sao không?

A: tại thời gian này, chỉ các ứng dụng hiện đại được liệt kê cho PC chạy Windows 10 được xác định là thiết bị của doanh nghiệp. InTune không thu thập thông tin về các ứng dụng Win32 cài đặt trên các thiết bị này.

Câu hỏi: tại sao các số điện thoại không được thu thập từ tất cả các thiết bị?

A: điện thoại phân loại là các thiết bị doanh nghiệp trong InTune không được xác định với số điện thoại đầy đủ của họ khi, ví dụ: bạn chạy báo cáo kho thiết bị di động. Mang theo-bạn-số điện thoại riêng của thiết bị luôn được che khuất một phần bằng dấu hoa thị (* * * *), và chỉ thể hiện bốn chữ số cuối cùng.