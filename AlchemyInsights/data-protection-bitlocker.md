---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118622"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Kích hoạt mã hóa Bitlocker với Intune

Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices. Để biết thêm thông tin, hãy [xem Windows 10 thiết đặt (trở lên) để bảo vệ thiết bị bằng cách sử dụng Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Ngoài Chính sách Bảo vệ Điểm cuối còn có một Báo cáo Mã hóa cung cấp dạng xem chi tiết hơn về trạng thái mã hóa cho thiết bị. Có thể truy nhập báo cáo này từ cổng thông tin MEM bên dưới **Thiết bị > Màn** hình, rồi bên dưới Cấu **hình, chọn** Báo cáo mã [hóa.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Nếu bạn thấy Bitlocker không được kích hoạt như mong đợi hoặc hồ sơ đang được sử dụng để bật Bitlocker đang ở trạng thái lỗi, vui lòng xem lại báo cáo mã hóa để hiểu rõ hơn về lý do tại sao hành vi lại xảy ra.

Để tìm chi tiết về cách diễn giải báo cáo bao gồm các giá trị trạng thái mã hóa khác nhau, hãy xem Mục Giám sát [mã hóa thiết bị với Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Bạn nên lưu ý rằng nhiều thiết bị mới hơn đang chạy Windows 10 hỗ trợ mã hóa Bitlocker tự động, được kích hoạt mà không cần ứng dụng chính sách MDM. Điều này có thể ảnh hưởng đến việc áp dụng chính sách nếu các thiết đặt không phải mặc định được cấu hình. Hãy xem câu hỏi thường gặp sau để biết thêm chi tiết.

Để biết thông tin về cách khắc phục sự cố bitlocker, hãy [xem Khắc phục sự cố chính sách BitLocker Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Câu hỏi thường gặp**

Hỏi: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng Chính sách Bảo vệ Điểm cuối?<br>
Đ: Các thiết đặt trong Chính sách Bảo vệ Điểm cuối Intune được thực thi bằng [cách sử dụng CSP Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Không phải tất cả các phiên bản hoặc bản dựng của Windows đều hỗ trợ CSP Bitlocker. <br><br>

Hỏi: Bitlocker có thể được bật như thế nào trên các thiết bị mà không yêu cầu tương tác với người dùng cuối?<br>
Đáp: Miễn là bạn đã đáp ứng các điều kiện tiên quyết cần thiết thì bạn vẫn có thể bật "Mã hóa Tĩnh" Bitlocker thông qua Intune. Xem chi tiết về các yêu cầu thiết bị và cài đặt chính sách mẫu để bật mã hóa im lặng trong tài liệu sau: Bật Mã hóa [Bitlocker một cách im lặng.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

Hỏi: Nếu một thiết bị đã được mã hóa bằng Bitlocker bằng các cài đặt mặc định của HĐH cho phương pháp mã hóa và độ bền mã hóa (XTS-AES-128), sẽ áp dụng một chính sách với các cài đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với các cài đặt mới?<br>
Hỏi: Không. Để áp dụng các thiết đặt mã hóa mới, ổ đĩa phải được giải mã trước tiên.<br><br>
**Lưu ý:** Đối với các thiết bị được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong quá trình OOBE không được kích hoạt cho đến khi chính sách Intune được đánh giá, cho phép sử dụng các thiết đặt dựa trên chính sách thay cho các mặc định HĐH.
 
Hỏi: Nếu một thiết bị được mã hóa do ứng dụng của chính sách Intune, thiết bị có được giải mã khi chính sách đó bị loại bỏ không?<br>
A: Việc loại bỏ chính sách liên quan đến mã hóa KHÔNG dẫn đến giải mã các ổ đĩa đã được cấu hình.
 
Hỏi: Tại sao Chính sách tuân thủ của Intune lại cho thấy thiết bị của tôi chưa bật Bitlocker, mặc dù đã được kích hoạt?<br>
Đ: Cài đặt "Bitlocker enabled" trong Chính sách Tuân thủ Intune sử dụng máy khách Windows Trạng trạng Thiết bị (DHA). Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động. Vì vậy, nếu một thiết bị chưa được khởi động lại kể từ khi mã hóa Bitlocker hoàn tất, dịch vụ máy khách DHA sẽ không báo cáo Bitlocker là hiện hoạt.
 
 