---
title: trình mô phỏng tấn công 2681 trong Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759241"
---
# <a name="attack-simulator-in-microsoft-365"></a>Trình mô phỏng tấn công trong Microsoft 365

- Bạn có thiếu mô phỏng tấn công không? Trình mô phỏng tấn công yêu cầu **office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** hoặc **Office 365 Enterprise E5**. Trình mô phỏng tấn công **không** được bao gồm trong Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, hoặc bất kỳ ứng dụng Microsoft 365 dành cho doanh nghiệp.

- Tài khoản mà bạn sử dụng để khởi động các cuộc tấn công mô phỏng yêu cầu người quản trị toàn cầu hoặc các quyền của người quản trị bảo mật và xác thực đa yếu tố (MFA). Để biết thêm thông tin về các yêu cầu về mô phỏng tấn công, hãy xem [chủ đề này](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Những điều quan trọng cần biết về các mô phỏng tấn công **mật khẩu Brute Force** :

  - Nếu tài khoản đích đã bật MFA và mật khẩu đã được đoán đúng, tài khoản sẽ không hiển thị là bị xâm phạm (yếu tố xác thực thứ hai sẽ không hoàn thành).

  - Tệp mật khẩu không thể lớn hơn 10 MB. Sử dụng một mật khẩu cho mỗi dòng, và bao gồm một đường trống (giao hàng trả về) sau khi mật khẩu cuối cùng trong danh sách.

- Những điều quan trọng cần biết về các mô phỏng về **lừa đảo** qua mạng:

  - Theo thiết kế, bạn không thể cung cấp giá trị tùy chỉnh cho **URL của máy chủ đăng nhập giả mạo**.

  - Nếu người nhận sử dụng phần [bổ trợ bật thông báo báo cáo](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) để báo cáo thư là lừa đảo, bạn có thể không nhận được cảnh báo cho thư (vì đây là một cuộc tấn công mô phỏng).

- Báo cáo: sau khi hoàn thành cuộc tấn công mô phỏng, bạn có thể bấm vào **chi tiết tấn công** để xem báo cáo.

- Để biết hướng dẫn chi tiết và các tính năng mới trong tấn công Simulator, hãy xem [tấn công Simulator trong Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
