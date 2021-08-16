---
title: Quy tắc giảm bề mặt tấn công
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 0f2e3d2d2cfa205f95a5d5dc84f7293fbee165a2976248de75a96379becd6925
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072218"
---
# <a name="attack-surface-reduction-rules"></a>Quy tắc giảm bề mặt tấn công

Loại trừ tệp hoặc thư mục có thể giảm nghiêm trọng bảo vệ do quy tắc giảm bề mặt tấn công cung cấp. Các tệp đã bị quy tắc cho phép chạy sẽ bị chặn và không có báo cáo hoặc sự kiện nào được ghi lại. Loại trừ áp dụng cho tất cả quy tắc cho phép loại trừ.

Loại trừ ASR sử dụng cùng một cú pháp như loại Tính năng Chống Virut của Bộ bảo vệ Microsoft loại trừ. Để biết chi tiết, [hãy xem Cấu hình và xác thực loại trừ cho Tính năng Chống Virut của Bộ bảo vệ Microsoft quét.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Để tránh vấn đề, [hãy xem lại Các lỗi phổ biến cần tránh khi xác định loại trừ.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Không phải tất cả quy tắc ASR đều hỗ trợ loại trừ. Để xác thực xem quy tắc của bạn có hỗ trợ loại trừ hay [không,](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)hãy xem bảng Các quy tắc giảm thiểu bề mặt tấn công .

## <a name="attack-surface-reduction-rules"></a>Quy tắc giảm bề mặt tấn công

Bề mặt tấn công của tổ chức bao gồm tất cả những nơi mà kẻ tấn công có thể xâm phạm thiết bị hoặc mạng của tổ chức. Giảm bề mặt tấn công của bạn đồng nghĩa với việc bảo vệ các thiết bị và mạng của tổ chức, điều này giúp những kẻ tấn công có ít cách thực hiện tấn công hơn. Cấu hình quy tắc giảm thiểu bề mặt tấn công trong Bộ bảo vệ Microsoft dành cho Điểm cuối có thể giúp ích.

Để biết thêm thông tin, hãy xem:

- [GUID quy tắc ánh xạ ASR thành tên](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Yêu cầu về quy tắc ASR:
    - [Windows 10 Pro, phiên bản 1709 trở lên](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, phiên bản 1709 trở lên](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Máy chủ, phiên bản 1803 (Kênh Nửa năm một lần) trở lên](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Xác định loại trừ chính xác cần áp dụng

1. Tìm kiếm EVENTID 1121 hoặc 1122 trong Microsoft-Windows-Bộ bảo vệ Windows/Nhật ký hoạt động.

1. Đánh giá kịch bản và ngữ cảnh của khối và xác nhận rằng kịch bản này cần được bỏ chặn.

1. Đọc giá trị Đường dẫn trong chi tiết sự kiện, là giá trị xác định loại trừ.
    - Thực hiện loại trừ càng nghiêm ngặt càng tốt.
    - Áp dụng ký tự đại diện mà cần (ví dụ: thay thế biến Người dùng).

1. Áp dụng loại trừ theo nhu cầu triển khai của bạn. Để biết chi tiết, xem mục [Tùy chỉnh quy tắc giảm thiểu bề mặt tấn công](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Loại trừ không được thực hiện

1. Xác định quy tắc có hỗ trợ loại trừ hay không. Để biết chi tiết, xem mục [Quy tắc giảm thiểu bề mặt tấn công](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Xem lại các loại trừ đã áp dụng và xác minh dữ liệu sự kiện về lỗi chính sách hoặc ký tự đại diện bị hiểu sai. Để biết thêm thông tin, hãy [xem Các loại loại trừ được hỗ trợ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. nếu ảnh hưởng của quy tắc đó quá cao, hãy xem xét việc di chuyển quy tắc (quay lại) sang chế độ Kiểm tra để thực hiện xác thực thêm. Để biết chi tiết, xem mục [Kiểm tra cách thức tính năng của Bộ bảo vệ Microsoft dành cho các tính năng Điểm cuối hoạt động trong chế độ kiểm tra](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Thu thập dữ liệu hỗ trợ để mở trường hợp hỗ trợ bằng cách sử dụng lệnh sau:
    
   ** MDEClientAnalyzer.cmd -v**

    Để biết thêm thông tin, hãy [xem mục Sự cố với máy tích hợp cho Bộ bảo vệ Microsoft dành cho Điểm cuối.](issues-with-onboarding-machines.md)
