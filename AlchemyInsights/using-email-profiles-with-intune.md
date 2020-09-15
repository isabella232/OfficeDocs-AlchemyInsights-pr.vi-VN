---
title: Sử dụng các hồ sơ email bằng InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653310"
---
# <a name="using-email-profiles-with-intune"></a>Sử dụng các hồ sơ email bằng InTune

InTune có thể được sử dụng để tạo và triển khai các hồ sơ email cho máy khách email gốc (tích hợp sẵn) trên nhiều nền tảng thiết bị.

Để biết thêm thông tin về một số hạn chế được liên kết với hồ sơ email, bao gồm cách xử lý các hồ sơ hiện có và cách loại bỏ hồ sơ email, hãy xem [Thêm thiết đặt email vào các thiết bị bằng cách dùng InTune](https://docs.microsoft.com/intune/email-settings-configure).

Để biết thêm thông tin về cách tạo hồ sơ email cho mỗi nền tảng thiết bị, hãy xem:

[Thiết đặt thiết bị Android để cấu hình email, xác thực và đồng bộ trong InTune](https://docs.microsoft.com/intune/email-settings-android)  
[Thêm thiết đặt email cho các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/email-settings-ios)  
[Thiết đặt hồ sơ email trong Microsoft InTune cho các thiết bị chạy Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Thiết đặt hồ sơ email cho các thiết bị chạy Windows 10 trong Microsoft InTune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Sự cố đồng bộ chung**

**Một KNOX trên hồ sơ email Android sẽ ngăn không cho người dùng liên hệ, lịch và tác vụ, từ các thiết bị của người dùng đang đồng bộ.**

Hồ sơ email của KNOX trên Android KNOX cung cấp tùy chọn quản trị để quyết định loại nội dung nào sẽ đồng bộ với thiết bị bằng cách đặt từng bật.

Nếu thiết đặt cho bất kỳ kiểu nội dung nào được đặt thành **không được cấu hình** (mặc định), thì kiểu nội dung đó không tự động đồng bộ. Người dùng có thể bật kiểu nội dung mà họ muốn trực tiếp trên thiết bị theo cách thủ công, nhưng cấu hình đó bị ghi đè bởi thiết đặt chính sách InTune và các điểm dừng đồng bộ cho kiểu nội dung đó.

