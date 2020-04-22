---
title: Điều khoản thiếu từ SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766875"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Cho phép mã hóa BitLocker với InTune

InTune Endpoint Protection chính sách có thể được sử dụng để cấu hình thiết đặt mã hóa Boitlocker cho các thiết bị Windows như được mô tả trong: Windows10 (và sau đó) cài đặt để bảo vệ thiết bị bằng cách sử dụng InTune

Bạn nên biết rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động được kích hoạt mà không có ứng dụng chính sách MDM. Điều này có thể ảnh hưởng đến áp dụng chính sách nếu không cài đặt mặc định được cấu hình. Xem FAQ để biết thêm chi tiết.


Câu  hỏi thường gặp Q: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng chính sách bảo vệ điểm cuối?
 A: cài đặt trong chính sách InTune Endpoint Protection được thực hiện bằng cách sử dụng CSP BitLocker.Không phải tất cả các phiên bản cũng không xây dựng Windows hỗ trợ CSP BitLocker. 
      Tại thời gian này phiên bản Windows: Enterprise; Giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (từ xây dựng 1809 trở đi) được hỗ trợ.




Câu hỏi: nếu thiết bị đã được mã hóa bằng BitLocker bằng cách sử dụng các thiết lập mặc định của hệ điều hành cho phương pháp mã hóa và cường độ (XTS-AES-128) sẽ áp dụng một chính sách với các cài đặt khác nhau tự động kích hoạt mã hóa lại ổ đĩa với các thiết đặt mới?

A: không. Để áp dụng các thiết lập mật mã mới, ổ đĩa đầu tiên phải được giải mã.

Lưu ý đối với các thiết bị được đăng ký với Autopilot mã hóa tự động sẽ xảy ra trong OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá cho phép chính sách dựa trên cài đặt được sử dụng ở nơi mặc định hệ điều hành




Câu hỏi: nếu thiết bị được mã hóa do ứng dụng chính sách InTune sẽ được giải mã khi chính sách đó bị xóa?

A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến giải mã các ổ đĩa được cấu hình.




Câu hỏi: tại sao chính sách tuân thủ dành cho thấy rằng thiết bị của tôi không có "đã bật BitLocker" nhưng?

A: cài đặt "bật BitLocker" trong chính sách tuân thủ InTune sử dụng máy khách chứng thực sự cố Windows Device (DHA). Máy khách này chỉ đo trạng thái thiết bị vào thời gian khởi động. Vì vậy, nếu một thiết bị không được khởi động lại kể từ khi mã hóa BitLocker đã hoàn thành dịch vụ khách hàng DHA sẽ không báo cáo BitLocker đang hoạt động.