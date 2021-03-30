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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405686"
---
# <a name="authentication-app"></a>Ứng dụng xác thực

Nếu bạn là người quản trị toàn cầu, bạn có thể nhanh chóng tìm hiểu điều gì đã xảy ra hoặc chẩn đoán các vấn đề liên quan đến người dùng đăng nhập bằng cách sử dụng [chẩn đoán đăng nhập](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Bắt đầu chẩn đoán bằng cách bấm nút "[khởi động chẩn đoán](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)". 
1. Tìm sự kiện để phân tích bằng cách nhập vào các chi tiết bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu ID hoặc tương quan ID.
1. Xem lại kết quả chẩn đoán Hiển thị chi tiết về những điều đã xảy ra và những hành động bạn có thể thực hiện để thay đổi, nếu bất kỳ thay đổi nào cần thiết.

**Kiểm tra tình huống được áp dụng:**

1. Nếu người dùng không nhận được thông báo đẩy trong ứng dụng Microsoft Authenticator, hãy xác minh rằng họ không được hiển thị bên dưới người dùng bị chặn MFA như được mô tả trong [khối và bỏ chặn người dùng](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Nếu người dùng không bị chặn đối với MFA nhưng không nhận được thông báo đẩy, họ có thể mở ứng dụng Microsoft Authenticator, vốn sẽ kéo các yêu cầu phê duyệt đang chờ xử lý.
1. Là phương pháp đăng nhập thay thế, người dùng cũng có thể bấm vào đăng nhập theo cách khác và chọn sử dụng mã xác minh từ ứng dụng dành cho thiết bị di động của tôi.
1. Ứng dụng Microsoft Authenticator là phương thức sẵn dùng duy nhất cho nhiều người dùng. [Tìm hiểu thêm về mặc định bảo mật](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), hãy chọn câu hỏi [thường gặp về ứng dụng](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) xác thực cho các câu hỏi thường gặp và cách giải quyết chúng.
 
**Video được đề xuất**

[Cách thiết lập ứng dụng Authenticator trên điện thoại mới (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
