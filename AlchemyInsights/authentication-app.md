---
title: Ứng dụng xác thực
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082964"
---
# <a name="authentication-app"></a>Ứng dụng xác thực

Nếu bạn là Người quản trị Toàn cầu, bạn có thể nhanh chóng tìm ra sự cố đã xảy ra hoặc chẩn đoán các sự cố liên quan đến đăng nhập người dùng bằng cách sử dụng Chẩn [đoán Đăng nhập.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Bắt đầu chẩn đoán bằng cách bấm vào nút "[Khởi chạy](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)chẩn đoán ". 
1. Tìm sự kiện cần phân tích bằng cách nhập các chi tiết mà bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu Id hoặc Id tương quan.
1. Xem lại kết quả chẩn đoán hiển thị chi tiết về sự cố đã xảy ra và những hành động bạn có thể thực hiện để thực hiện thay đổi, nếu cần bất kỳ thay đổi nào.

**Kiểm tra kịch bản có thể áp dụng:**

1. Nếu người dùng không nhận được thông báo đẩy trong ứng dụng Microsoft Authenticator, hãy xác minh rằng thông báo đó không hiển thị bên dưới MFA đã chặn người dùng như được mô tả trong Chặn và bỏ chặn người [dùng.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Nếu người dùng không bị chặn đối với MFA nhưng không nhận được thông báo đẩy, họ có thể mở ứng dụng Microsoft Authenticator, việc này sẽ kéo các yêu cầu phê duyệt đang chờ xử lý.
1. Như một phương thức đăng nhập thay thế, người dùng cũng có thể bấm vào Đăng nhập bằng cách khác và chọn sử dụng mã xác minh từ ứng dụng dành cho thiết bị di động của tôi.
1. Ứng Microsoft Authenticator là phương pháp duy nhất sẵn dùng đối với nhiều người dùng. [Tìm hiểu thêm về các mặc định bảo mật](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), hãy Authenticator câu hỏi [thường](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) gặp về Ứng dụng để biết các câu hỏi thường gặp và cách giải quyết các câu hỏi này.
 
**Video được Đề xuất**

[Cách thiết lập Authenticator App trên điện thoại mới (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
