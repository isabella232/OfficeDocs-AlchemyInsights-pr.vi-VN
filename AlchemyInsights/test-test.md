---
title: Thiếu thuật ngữ trong Kho Thuật SharePoint Trực tuyến
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106454"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Kích hoạt Mã hóa BitLocker với Intune

Bạn có thể sử dụng Chính sách Bảo vệ Điểm cuối của Intune để đặt cấu hình cài đặt mã hóa Boitlocker cho Windows như được mô tả trong : Cài đặt Windows10 (trở lên) để bảo vệ thiết bị bằng Intune

Bạn nên lưu ý rằng nhiều thiết bị mới hơn đang chạy Windows 10 hỗ trợ mã hóa bitlocker tự động được kích hoạt mà không cần ứng dụng chính sách MDM. Điều này có thể ảnh hưởng đến việc áp dụng chính sách nếu cài đặt không phải mặc định được cấu hình. Hãy xem Câu hỏi thường gặp để biết thêm chi tiết.


Câu hỏi thường gặp: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng Chính sách Bảo vệ Điểm cuối?
Đ: Các thiết đặt trong Chính sách Bảo vệ Điểm cuối Intune được thực thi bằng cách sử dụng CSP Bitlocker.  Không phải tất cả các phiên bản cũng như bản dựng của Windows hỗ trợ CSP Bitlocker. Tại thời điểm này Windows phiên bản: Doanh nghiệp; Giáo dục, Di động, Doanh nghiệp Di động và Chuyên nghiệp (từ bản dựng 1809 trở lên) được hỗ trợ.




Hỏi: Nếu một thiết bị đã được mã hóa bằng Bitlocker bằng cài đặt mặc định của HĐH cho phương pháp mã hóa và giới từ mã hóa (XTS-AES-128) sẽ áp dụng chính sách với các cài đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với cài đặt mới không?

Hỏi: Không. Để áp dụng các cài đặt mã lệnh mới, trước tiên ổ đĩa phải được giải mã.

Lưu ý Đối với các thiết bị được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong quá trình OOBE không được kích hoạt cho đến khi chính sách Intune được đánh giá, cho phép sử dụng các cài đặt dựa trên chính sách thay cho mặc định HĐH




Hỏi Nếu một thiết bị được mã hóa do việc áp dụng chính sách Intune, thiết bị đó sẽ được giải mã khi chính sách đó bị loại bỏ?

A: Việc loại bỏ chính sách mã hóa liên quan không dẫn đến giải mã các ổ đĩa đã được cấu hình.




Hỏi: Tại sao chính sách tuân thủ của intune lại cho thấy rằng thiết bị của tôi không bật "Bitlocker Đã bật" nhưng chính sách này là?

Đ: Cài đặt "Bitlocker đã bật" trong chính sách tuân thủ intune sử dụng máy khách Windows chứng tình trạng thiết bị (DHA). Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động. Vì vậy, nếu một thiết bị chưa được khởi động lại kể từ khi mã hóa bitlocker hoàn tất, dịch vụ máy khách DHA sẽ không báo cáo bitlocker khi hiện hoạt.