---
title: Các thuật ngữ bị thiếu trong lưu trữ thuật ngữ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750473"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bật tính năng mã hóa BitLocker bằng InTune

Có thể sử dụng chính sách bảo vệ Endpoint trong InTune để cấu hình thiết đặt mã hóa Boitlocker cho các thiết bị Windows như được mô tả trong: Windows10 (và phiên sau) để bảo vệ các thiết bị bằng cách dùng InTune

Bạn nên lưu ý rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động được kích hoạt mà không cần áp dụng chính sách MDM. Việc này có thể tác động đến ứng dụng chính sách nếu thiết đặt mặc định không được cấu hình. Xem câu hỏi thường gặp về chi tiết hơn.


Câu hỏi thường gặp   hỏi: Phiên bản nào của mã hóa thiết bị hỗ trợ Windows bằng chính sách bảo vệ điểm cuối?
 A: các thiết đặt trong chính sách bảo vệ điểm cuối trong InTune được thực hiện bằng cách sử dụng CPC BitLocker.Không phải tất cả các phiên bản cũng không phải là bản dựng của Windows hỗ trợ CPC BitLocker. 
      Tại phiên bản Windows thời gian này: Enterprise; Giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (từ bản dựng 1809 trở đi) được hỗ trợ.




Hỏi: nếu thiết bị đã được mã hóa với BitLocker bằng cách dùng thiết đặt mặc định của hệ điều hành cho phương pháp mã hóa và sức mạnh của mật độ (XTS-AES-128) sẽ áp dụng chính sách với các thiết đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với cài đặt mới?

A: không. Để áp dụng các thiết đặt mã hóa mới, trước tiên, bạn phải được giải mã.

Lưu ý đối với các thiết bị đang được đăng ký với Autopilot mã hóa tự động sẽ xảy ra trong khi OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá cho phép các thiết đặt dựa trên chính sách sẽ được sử dụng thay cho mặc định của hệ điều hành




Hỏi nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune sẽ được giải mã khi chính sách đó bị loại bỏ?

A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến việc giải mã các ổ đĩa được cấu hình.




Hỏi: tại sao không điều chỉnh chính sách tuân thủ cho biết thiết bị của tôi không có "BitLocker đã bật" nhưng nó là gì?

A: thiết đặt "BitLocker Enabled" trong chính sách tuân thủ InTune sẽ sử dụng máy khách Attestation (DHA) của thiết bị Windows (DHA). Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động. Vì vậy, nếu thiết bị không được khởi động lại từ khi mã hóa BitLocker đã hoàn tất dịch vụ máy khách DHA sẽ không báo cáo BitLocker khi đang hiện hoạt.