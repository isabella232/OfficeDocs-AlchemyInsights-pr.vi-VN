---
title: Sử dụng hồ sơ email với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555756"
---
# <a name="using-email-profiles-with-intune"></a>Sử dụng hồ sơ email với InTune

InTune có thể được sử dụng để tạo và triển khai hồ sơ email cho máy khách email gốc (tích hợp) trên nhiều nền tảng thiết bị.

Để biết thông tin về một số hạn chế liên quan đến hồ sơ email, bao gồm cách xử lý sự hiện diện của các cấu hình hiện có và cách xóa hồ sơ email, hãy xem [Thêm cài đặt email vào thiết bị bằng InTune](https://docs.microsoft.com/intune/email-settings-configure).

Để biết thêm thông tin về cách tạo hồ sơ email cho từng nền tảng thiết bị, xem:

[Cài đặt thiết bị Android để đặt cấu hình email, xác thực và đồng bộ hoá trong InTune](https://docs.microsoft.com/intune/email-settings-android)  
[Thêm cài đặt e-mail cho các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/email-settings-ios)  
[Cài đặt cấu hình email trong Microsoft InTune cho các thiết bị chạy Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Cài đặt cấu hình email cho các thiết bị chạy Windows 10 trong Microsoft InTune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vấn đề đồng bộ hoá phổ biến**

**Một KNOX trên hồ sơ email Android ngăn người dùng liên hệ, lịch và tác vụ, từ đang được đồng bộ với thiết bị người dùng.**

KNOX trên hồ sơ email Android KNOX cung cấp quản trị tùy chọn để quyết định loại nội dung nào đang đồng bộ hóa với thiết bị bằng cách đặt từng bật.

Nếu cài đặt cho bất kỳ loại nội dung nào được đặt thành **không cấu hình** (mặc định), loại nội dung đó không đồng bộ tự động. Người dùng có thể kích hoạt loại nội dung mà họ muốn trực tiếp trên thiết bị theo cách thủ công, nhưng cấu hình đó được ghi đè bởi thiết đặt chính sách InTune và dừng đồng bộ hóa cho loại nội dung đó.

