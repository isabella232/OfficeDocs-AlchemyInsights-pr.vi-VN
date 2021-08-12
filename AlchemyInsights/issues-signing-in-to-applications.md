---
title: Các sự cố về đăng nhập vào ứng dụng
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
ms.openlocfilehash: e1fd31366f24331e74b7e35887c3275549a7a394b128da560ba7a76437979553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925691"
---
# <a name="issues-signing-in-to-applications"></a>Các sự cố về đăng nhập vào ứng dụng

Để phát hiện nguyên nhân hoặc chẩn đoán các vấn đề liên quan đến đăng nhập người dùng, hãy thực hiện các bước sau đây:

1. Khởi chạy [Chẩn đoán Đăng nhập.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
2. Tìm sự kiện cần phân tích bằng cách nhập thông tin chi tiết về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu Id hoặc Id tương quan.
3. Xem lại kết quả chẩn đoán hiển thị chi tiết về sự cố đã xảy ra và những hành động bạn có thể thực hiện để thực hiện thay đổi, nếu cần bất kỳ thay đổi nào.

Sau đây là một số sự cố phổ biến bạn có thể gặp phải khi đăng nhập vào ứng dụng:

1. Bạn hoặc người dùng đã hoàn tất đăng nhập **Azure AD** [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) nhưng đang thấy lời nhắc ngoài dự kiến - Xem các bài viết Lời nhắc chấp thuận không mong muốn khi đăng nhập vào ứng dụng và Lỗi không mong muốn khi thực hiện đồng ý với ứng dụng [.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
2. Bạn hoặc người dùng đã đăng nhập trực tiếp vào một ứng dụng **nhưng** không thể đăng nhập vào ứng dụng đó từ một liên kết sâu trên cổng thông tin tùy chỉnh hoặc panel truy nhập : Xem mục Khắc phục sự cố khi đăng nhập vào ứng dụng từ [Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Bạn hoặc người dùng đã hoàn tất đăng nhập **Azure AD** nhưng ứng dụng sẽ hiển thị thông báo lỗi và không cho phép người dùng hoàn tất dòng đăng nhập : Sự cố là ứng dụng đã không chấp nhận phản hồi mà Azure AD phát hành. Hãy làm theo [các bước sau để](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) khắc phục sự cố.
4. Bạn hoặc người dùng **không** thể đăng nhập vào một ứng dụng không phải là bộ sưu tập được cấu hình để đăng nhập một lần bằng mật khẩu: Hãy làm theo hướng dẫn trong các bước sau để [khắc](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) phục sự cố.
5. Bạn hoặc người dùng không thể đăng nhập vào một ứng dụng Bộ sưu **tập Azure AD** được đặt cấu hình cho đăng nhập một lần bằng mật khẩu: Hãy làm theo các bước sau để [khắc](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) phục sự cố.
6. Bạn hoặc người dùng không **thể đăng nhập vào một ứng dụng của Microsoft: Hãy** làm theo các bước sau để [khắc](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) phục sự cố.
7. Bạn hoặc người dùng **không** thể đăng nhập vào một ứng dụng không phải là bộ sưu tập được cấu hình cho đăng nhập đơn được liên kết: Hãy làm theo các bước sau [để](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) khắc phục sự cố.
8. Bạn hoặc người dùng không thể đăng nhập vào một ứng dụng Bộ sưu **tập Azure AD** được đặt cấu hình cho đăng nhập đơn được liên kết: Hãy làm theo các bước sau [để](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) khắc phục sự cố.
9. Bạn hoặc người dùng không **thể đăng nhập vào một ứng dụng tùy chỉnh phát** triển: Hãy làm theo các [bước sau để khắc](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) phục sự cố.
10. Bạn hoặc người dùng không thể đăng nhập vào một ứng dụng tại cơ sở bằng proxy ứng dụng **Azure AD: Hãy làm** theo các bước sau để [khắc](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) phục sự cố.

