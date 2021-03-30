---
title: Trình quản lý điểm cuối-đường cơ sở bảo mật
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421219"
---
# <a name="endpoint-manager---security-baselines"></a>Trình quản lý điểm cuối-đường cơ sở bảo mật

Các cấu hình bảo mật được các nhóm thiết đặt sẵn của Windows giúp bạn áp dụng các thiết đặt bảo mật được đề xuất bởi nhóm bảo mật liên quan. Những đường kết nối này có thể được tùy chỉnh để chỉ cung cấp các thiết đặt và giá trị mong muốn. Để biết thêm thông tin về cấu hình bảo mật, hãy xem sử dụng các máy tính [bảo mật để cấu hình thiết bị chạy Windows 10 trong InTune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Hiện tại có những đường cơ sở cho những sản phẩm này:

- Thiết đặt bảo mật Windows MDM
- Microsoft Defender cho bảo mật điểm cuối
- Microsoft Edge

Mỗi đường cơ sở được Cập Nhật theo định kỳ và được phát hành trong các phiên bản gia tăng. Mỗi phiên bản thêm và loại bỏ các thiết đặt từ phiên bản trước đó để đảm bảo rằng đường cơ sở gặp phải hướng dẫn hiện tại. Giao diện người dùng bảo mật trong Endpoint Security cho phép các phiên bản khác nhau được so sánh bằng cách thực hiện các thay đổi từ phiên bản sang phiên bản Hiển thị.

Để biết hướng dẫn về cách thay đổi hiệu quả nhất mà phiên bản của đường cơ sở được triển khai, hãy xem [quản lý hồ sơ đường cơ sở bảo mật trong Microsoft InTune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Sau khi triển khai một đường cơ sở bảo mật, bạn có thể theo dõi các thiết đặt trạng thái triển khai và xem lại trên cơ sở thiết bị theo từng thiết bị.

**Lưu ý:** Dữ liệu báo cáo cho các máy tính có thể mất tối đa 24 giờ để xuất hiện từ triển khai ban đầu cho một thiết bị và tối đa 6 giờ để biết thêm các bản Cập Nhật. 

Nguyên nhân phổ biến nhất của một thiết đặt đường cơ sở không áp dụng được vì cùng một thiết đặt đang được dùng trong một hồ sơ khác. Tình huống này có thể được điều tra cho thiết bị cụ thể bằng cách chọn thiết bị đó từ bên trong nút trạng thái thiết bị của hồ sơ cơ sở bảo mật. Để biết chi tiết, hãy xem [giải quyết xung đột cho](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)các đường cơ sở bảo mật.