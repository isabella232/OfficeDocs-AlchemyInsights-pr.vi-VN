---
title: Thiết đặt SMTP cho Microsoft 365 vụ thư
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813987"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Thiết đặt SMTP cho Microsoft 365 vụ thư

Đây là các thiết đặt SMTP cho người Microsoft 365 vụ thư:

**Máy** chủ : smtp.office365.com </br>
**Cổng**: 587 </br>
**Mã** hóa : STARTTLS (Giờ đây chỉ hỗ trợ phiên bản TLS 1.2. Vui lòng đảm bảo rằng ứng dụng hoặc thiết bị của bạn hỗ trợ TLS 1.2) </br>
**Tên** người dùng : Địa Office 365 Của bạn (ví dụ: example@yourdomain.com) </br>
**Mật khẩu**: Mật khẩu tài Office 365 bạn </br>
**Xác thực**: Bắt buộc </br>
**Giới hạn** gửi : 10.000 email/ngày </br>

Để biết thiết đặt POP và IMAP, hãy [xem Thiết đặt POP, IMAP và SMTP.](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)
 
Để tìm hiểu về các tùy chọn chuyển tiếp email bằng Microsoft 365 và các bước, hãy xem Cách thiết lập ứng dụng hoặc thiết bị đa năng để gửi email bằng Microsoft 365 hoặc [Office 365.](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)