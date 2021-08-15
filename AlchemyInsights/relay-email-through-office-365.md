---
title: Chuyển tiếp email qua Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024228"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Thiết lập ứng dụng hoặc thiết bị đa năng để gửi email

Để tìm hiểu về các tùy chọn và các bước, xem mục Cách thiết lập thiết bị đa năng hoặc ứng dụng để [gửi email bằng](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)Microsoft 365.
  
Nếu bạn có một thiết bị hoặc ứng dụng mà gần đây đã ngừng hoạt động, các vấn đề phổ biến nhất là:

- **Xác thực các lỗi liên quan đến xác thực trong khi sử dụng bản gửi máy khách SmTP Auth** Gần đây, chúng tôi đã thực hiện một số thay đổi liên quan đến cách thức hoạt động của Xác thực SMTP. Để biết thêm thông tin về cách giải quyết sự cố, hãy xem mục xác thực không thành công trong mục Khắc phục sự cố với máy in, máy quét và ứng dụng LOB gửi email bằng Microsoft 365 hoặc [máy Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Chúng tôi chỉ chấp nhận phiên bản TLS 1.2 trong khi tạo kết nối bảo mật để truy Office 365** Nếu bạn đang sử dụng Kết nối bảo mật (TLS), hãy đảm bảo thiết bị ứng dụng của bạn hỗ trợ TLS 1.2. Để biết thêm thông tin, [hãy xem chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Để biết các sự cố và giải pháp khác, hãy xem mục Khắc phục sự cố với máy in, máy quét và các ứng dụng LOB gửi email bằng Microsoft 365 hoặc [Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Để xem các thiết bị bị ảnh hưởng, hãy đi đến [báo cáo Máy khách Xác thực SMTP.](https://protection.office.com/mailflow/dashboard)

**Lưu** ý : Exchange Online không phù hợp với tình huống gửi thư hàng loạt. Để gửi email thương mại hàng loạt (ví dụ: bản tin khách hàng), bạn nên sử dụng các nhà cung cấp bên thứ ba chuyên về các dịch vụ này.
