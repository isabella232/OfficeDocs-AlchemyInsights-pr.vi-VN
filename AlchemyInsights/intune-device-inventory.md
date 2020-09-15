---
title: Kiểm kê thiết bị InTune
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667900"
---
# <a name="intune-device-inventory"></a>Kiểm kê thiết bị InTune

Blade thiết bị cung cấp cho người quản trị hiểu sâu vào các thiết bị dưới quản lý trong InTune trên mỗi cơ sở thiết bị. Thông tin được hiển thị bao gồm: phần cứng, ứng dụng đã phát hiện, trạng thái tuân thủ thiết bị và trạng thái cấu hình thiết bị.

Dữ liệu hàng tồn kho cho phần cứng và các ứng dụng được phát hiện được thu thập trong vòng tròn bảy ngày. Các ứng dụng và phần cứng cụ thể được báo cáo khác nhau tùy thuộc vào hệ điều hành thiết bị và liệu thiết bị có cá nhân hoặc công ty thuộc sở hữu.

Để biết thêm thông tin, hãy xem [xem chi tiết thiết bị trong InTune](https://docs.microsoft.com/intune/device-inventory).

**DIỄN**

Hỏi: tôi không nhận được danh sách các ứng dụng hàng tồn kho đầy đủ trình bày trên thiết bị Windows được đăng ký theo dõi. Tại sao không?

A: tại thời điểm này, chỉ các ứng dụng hiện đại được liệt kê cho PC chạy Windows 10 được xác định là các thiết bị công ty. InTune không thu thập thông tin về các ứng dụng Win32 được cài đặt trên các thiết bị này.

Hỏi: tại sao số điện thoại không được thu thập từ tất cả các thiết bị?

A: điện thoại được phân loại là các thiết bị công ty trong InTune không được xác định bằng số điện thoại đầy đủ của họ khi, ví dụ: bạn chạy báo cáo kiểm kê trên thiết bị di động. Mang theo-bạn-riêng-các số điện thoại của thiết bị luôn là một phần masked với các dấu sao (* * * *) và chỉ hiện bốn chữ số cuối cùng.