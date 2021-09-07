---
title: Trình quản lý Điểm cuối - Đường cơ sở bảo mật
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
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923576"
---
# <a name="endpoint-manager---security-baselines"></a>Trình quản lý Điểm cuối - Đường cơ sở bảo mật

Đường cơ sở bảo mật là các nhóm thiết đặt Windows cấu hình trước để giúp bạn áp dụng các thiết đặt bảo mật mà các nhóm bảo mật liên quan đề xuất. Các đường cơ sở này có thể được tùy chỉnh để chỉ cung cấp các thiết đặt và giá trị mong muốn. Để biết thêm thông tin về đường cơ sở bảo mật, hãy xem mục Sử dụng đường cơ sở bảo mật [để đặt cấu Windows 10 thiết bị trong Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Hiện có các đường cơ sở cho các sản phẩm này:

- Windows Thiết đặt Bảo mật MDM
- Bộ bảo vệ Microsoft dành cho Bảo mật Điểm cuối
- Microsoft Edge

Mỗi đường cơ sở được cập nhật định kỳ và phát hành theo phiên bản tăng dần. Mỗi phiên bản thêm và hoặc loại bỏ cài đặt khỏi phiên bản trước nhằm đảm bảo rằng đường cơ sở đáp ứng hướng dẫn hiện tại. Bảng điều khiển Đường cơ sở bảo mật trong Bảo mật Điểm cuối cho phép so sánh các phiên bản khác nhau bằng cách hiển thị các thay đổi từ phiên bản này sang phiên bản khác.

Để biết hướng dẫn về cách triển khai phiên bản đường cơ sở hiệu [quả nhất,](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)hãy xem mục Quản lý hồ sơ đường cơ sở bảo mật Microsoft Intune .

Sau khi triển khai một đường cơ sở bảo mật, bạn có thể theo dõi trạng thái triển khai và xem xét thiết đặt trên cơ sở từng thiết bị.

Vì đường cơ sở bảo mật chứa nhiều thiết đặt, điều quan trọng là phải xem lại những thay đổi về cấu hình và thực hiện kiểm tra để đảm bảo tất cả các thiết đặt đều thích hợp cho các thiết bị và nhu cầu kinh doanh của bạn.

**Lưu ý:** Dữ liệu báo cáo cho đường cơ sở có thể mất đến 24 giờ để xuất hiện từ lần triển khai ban đầu đến một thiết bị và tối đa 6 giờ để cập nhật thêm. 

Nguyên nhân phổ biến nhất của thiết đặt đường cơ sở không áp dụng là vì cùng một thiết đặt đang được sử dụng trong một hồ sơ khác. Kịch bản này có thể được điều tra cho thiết bị cụ thể bằng cách chọn thiết bị đó từ bên trong nút Trạng thái Thiết bị của hồ sơ Đường cơ sở Bảo mật. Để biết chi tiết, [hãy xem Giải quyết xung đột cho đường cơ sở bảo mật](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).