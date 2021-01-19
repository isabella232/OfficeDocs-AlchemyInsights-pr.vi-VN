---
title: Các sự cố khi đăng nhập vào ứng dụng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901320"
---
# <a name="issues-signing-in-to-applications"></a>Các sự cố khi đăng nhập vào ứng dụng

Để phát hiện nguyên nhân hoặc chẩn đoán các vấn đề liên quan đến đăng nhập người dùng, hãy thực hiện các bước sau đây:

1. Khởi động [chẩn đoán đăng nhập](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Tìm sự kiện để phân tích bằng cách nhập các chi tiết mà bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu ID hoặc tương quan ID.
3. Xem lại kết quả chẩn đoán Hiển thị chi tiết về những điều đã xảy ra và những hành động bạn có thể thực hiện để thay đổi, nếu bất kỳ thay đổi nào cần thiết.

Sau đây là một số vấn đề phổ biến mà bạn có thể gặp phải khi đăng nhập vào các ứng dụng:

1. Bạn hoặc người dùng **đã hoàn thành một đăng nhập AZURE AD, nhưng đang nhìn thấy lời nhắc bất ngờ** -xem các bài viết [chấp thuận không mong muốn khi đăng nhập vào một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) và [lỗi không mong muốn khi thực hiện đồng ý với một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Bạn hoặc người dùng **đã đăng nhập trực tiếp vào một ứng dụng, nhưng không thể đăng nhập vào tài liệu đó từ một trang chiếu trên cổng tùy chỉnh hoặc Panel Access**: xem [khắc phục sự cố đăng nhập vào một ứng dụng từ Azure AD ứng dụng của tôi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Bạn hoặc người dùng **đã hoàn thành một đăng nhập AZURE AD, nhưng ứng dụng sẽ hiển thị thông báo lỗi và không cho phép người dùng hoàn tất dòng đăng nhập**: vấn đề là ứng dụng đó không chấp nhận phản hồi phát hành Azure AD. Hãy làm theo [các bước sau](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) để khắc phục sự cố.
4. Bạn hoặc người dùng **không thể đăng nhập vào ứng dụng không phải bộ sưu tập được đặt cấu hình cho đăng nhập bằng mật khẩu**: làm theo hướng dẫn trong [các bước sau](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) để khắc phục sự cố.
5. Bạn hoặc người dùng **không thể đăng nhập vào ứng dụng AZURE AD Gallery được đặt cấu hình cho đăng nhập đơn**: làm theo [các bước sau đây](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) để khắc phục sự cố.
6. Bạn hoặc người dùng **không thể đăng nhập vào một ứng dụng Microsoft**: làm theo [các bước sau](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) để khắc phục sự cố.
7. Bạn hoặc người dùng **không thể đăng nhập vào một ứng dụng không phải bộ sưu tập được đặt cấu hình cho đăng nhập đơn**: làm theo [các bước sau](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) để khắc phục sự cố.
8. Bạn hoặc người dùng **không thể đăng nhập vào ứng dụng AZURE AD Gallery được đặt cấu hình cho đăng nhập đơn**: làm theo [các bước sau đây](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) để khắc phục sự cố.
9. Bạn hoặc người dùng **không thể đăng nhập vào một ứng dụng được phát triển tùy chỉnh**: Hãy làm theo [các bước sau](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) để khắc phục sự cố.
10. Bạn hoặc người dùng **không thể đăng nhập vào một ứng dụng tại chỗ bằng proxy ứng dụng AZURE AD**: làm theo [các bước sau đây](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) để khắc phục sự cố.

