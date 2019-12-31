---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908731"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Cho phép mã hóa BitLocker với InTune

 Chính sách bảo vệ điểm cuối InTune có thể được sử dụng để cấu hình cài đặt mã hóa BitLocker cho thiết bị Windows. Để biết thêm thông tin, xem [cài đặt Windows 10 (và sau này) để bảo vệ thiết bị bằng cách sử dụng InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Bạn nên biết rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động, được kích hoạt mà không có ứng dụng chính sách MDM. Điều này có thể ảnh hưởng đến áp dụng chính sách nếu thiết đặt không mặc định được cấu hình. Xem FAQ sau đây để biết thêm chi tiết.
 
Để biết thông tin về khắc phục sự cố BitLocker, xem [khắc phục sự cố chính sách BitLocker trong Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 Câu hỏi: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng chính sách bảo vệ điểm cuối?<br>
 A: cài đặt trong chính sách bảo vệ điểm cuối được thực hiện bằng cách sử dụng [CSP BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Không phải tất cả các phiên bản hoặc xây dựng Windows hỗ trợ CSP BitLocker. <br><br>
      Tại thời gian này, các phiên bản Windows sau được hỗ trợ: doanh nghiệp, giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (xây dựng 1809 và mới hơn).
 
Câu hỏi: nếu một thiết bị đã được mã hóa bằng BitLocker bằng cách sử dụng các thiết lập mặc định hệ điều hành cho phương pháp mã hóa và cường độ (XTS-AES-128), sẽ áp dụng một chính sách với các cài đặt khác nhau tự động kích hoạt mã hóa lại ổ đĩa với các cài đặt mới?<br>
A: không. Để áp dụng cài đặt mật mã mới, ổ đĩa trước tiên phải được giải mã.<br><br>
**Lưu ý:** Đối với các thiết bị được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá, cho phép các thiết đặt dựa trên chính sách được sử dụng tại chỗ của hệ điều hành mặc định.
 
Câu hỏi: nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune, nó sẽ được giải mã khi chính sách đó bị xóa?<br>
A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến giải mã ổ đĩa được cấu hình.
 
Câu hỏi: tại sao chính sách tuân thủ InTune cho thấy rằng thiết bị của tôi không bật BitLocker, mặc dù nó là?<br>
A: cài đặt "bật BitLocker" trong chính sách tuân thủ InTune sử dụng máy khách chứng thực tình trạng Windows Device (DHA). Máy khách này chỉ đo trạng thái thiết bị vào thời gian khởi động. Vì vậy, nếu một thiết bị không được khởi động lại kể từ khi mã hóa BitLocker được hoàn thành, Dịch vụ khách hàng DHA sẽ không báo cáo BitLocker đang hoạt động.
 
 