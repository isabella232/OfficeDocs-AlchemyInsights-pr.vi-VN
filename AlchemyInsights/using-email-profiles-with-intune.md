---
title: Sử dụng hồ sơ email với Intune
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919445"
---
# <a name="using-email-profiles-with-intune"></a>Sử dụng hồ sơ email với Intune

Intune có thể được sử dụng để tạo và triển khai hồ sơ email cho máy khách email gốc (tích hợp sẵn) trên nhiều nền tảng thiết bị.

Để biết thông tin về một số hạn chế liên kết với hồ sơ email, bao gồm cách xử lý sự hiện diện của hồ sơ hiện có và cách loại bỏ hồ sơ email, hãy xem Thêm thiết đặt email vào thiết bị bằng cách sử dụng [Intune](https://docs.microsoft.com/intune/email-settings-configure).

Để biết thêm thông tin về cách tạo hồ sơ email cho mỗi nền tảng thiết bị, hãy xem:

[Cài đặt thiết bị Android để đặt cấu hình email, xác thực và đồng bộ hóa trong Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Thêm cài đặt email cho thiết bị iOS và iPadOS trong Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Thiết đặt hồ sơ email Microsoft Intune cho thiết bị chạy Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Thiết đặt hồ sơ email cho thiết bị chạy Windows 10 trong Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Sự cố đồng bộ phổ biến**

**Cấu hình email KNOX trên Android sẽ ngăn không cho liên hệ, Lịch và Tác vụ của người dùng đồng bộ với các thiết bị người dùng.**

Hồ sơ email KNOX trên Android KNOX cung cấp cho người quản trị tùy chọn để quyết định loại nội dung được đồng bộ với thiết bị bằng cách đặt từng loại nội dung được bật.

Nếu thiết đặt cho bất kỳ kiểu nội dung nào được đặt là Không được cấu hình **(mặc** định), thì kiểu nội dung đó không tự động đồng bộ. Người dùng có thể bật loại nội dung họ muốn trực tiếp trên thiết bị theo cách thủ công nhưng cấu hình đó bị ghi đè bởi cài đặt chính sách Intune và đồng bộ sẽ ngừng cho loại nội dung đó.

