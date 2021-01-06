---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768839"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bật tính năng mã hóa BitLocker bằng InTune

 Có thể sử dụng chính sách bảo vệ Endpoint trong InTune để cấu hình thiết đặt mã hóa BitLocker cho các thiết bị chạy Windows. Để biết thêm thông tin, hãy xem [thiết đặt Windows 10 (và mới hơn) để bảo vệ các thiết bị bằng cách dùng InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Bạn nên lưu ý rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động, được kích hoạt mà không có ứng dụng của chính sách MDM. Điều này có thể tác động đến ứng dụng chính sách nếu thiết đặt không phải mặc định được cấu hình. Xem câu hỏi thường gặp sau đây để biết thêm chi tiết.
 
Để biết thông tin về khắc phục sự cố BitLocker, hãy xem [khắc phục sự cố chính sách BitLocker trong Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**DIỄN**

Hỏi: Phiên bản nào của mã hóa thiết bị hỗ trợ Windows sử dụng chính sách bảo vệ điểm cuối?<br>
A: các thiết đặt trong chính sách bảo vệ điểm cuối trong InTune được thực hiện bằng cách sử dụng [CPC BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Không phải tất cả các phiên bản hoặc bản dựng của Windows hỗ trợ CPC BitLocker. <br><br>

Hỏi: có thể bật BitLocker trên các thiết bị mà không yêu cầu người dùng cuối tương tác?<br>
A: miễn là các site trước cần thiết được đáp ứng có thể bật BitLocker "mã hóa im lặng" thông qua InTune. Xem chi tiết về các yêu cầu thiết bị và các thiết đặt chính sách ví dụ để bật mã hóa im lặng trong tài liệu sau đây: âm thanh cho [phép mã hóa BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Hỏi: nếu thiết bị đã được mã hóa với BitLocker bằng cách dùng thiết đặt mặc định của hệ điều hành cho phương pháp mã hóa và sức mạnh của mật độ (XTS-AES-128), sẽ áp dụng chính sách với các thiết đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với cài đặt mới?<br>
A: không. Để áp dụng các thiết đặt mã hóa mới, trước tiên, ổ đĩa phải được giải mã.<br><br>
**Lưu ý:** Đối với các thiết bị đang được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong khi OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá, cho phép các thiết đặt dựa trên chính sách sẽ được sử dụng thay cho mặc định của hệ điều hành.
 
Hỏi: nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune, nó sẽ được giải mã khi chính sách đó bị loại bỏ?<br>
A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến việc giải mã các ổ đĩa đã được cấu hình.
 
Hỏi: tại sao không điều chỉnh chính sách tuân thủ cho biết thiết bị của tôi không được bật BitLocker, ngay cả khi có hiệu lực đó?<br>
A: thiết đặt "BitLocker Enabled" trong chính sách tuân thủ InTune sẽ áp dụng máy khách Attestation (DHA) của thiết bị Windows (DHA). Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động. Vì vậy, nếu thiết bị không được khởi động lại từ khi mã hóa BitLocker đã được hoàn tất, Dịch vụ máy khách DHA sẽ không báo cáo BitLocker khi đang hiện hoạt.
 
 