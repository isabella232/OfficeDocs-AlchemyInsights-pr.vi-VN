---
title: Vấn đề phát triển ứng dụng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013446"
---
# <a name="issues-developing-applications"></a>Vấn đề phát triển ứng dụng

Để khắc phục các sự cố phổ biến nhất khi xây dựng Azure Active Directory dụng (AD), hãy xem các bài viết sau đây:

- [Tôi gặp sự cố khi đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Tôi không biết cách thay đổi mặc định thời hạn mã thông báo cho ứng dụng của mình](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Tôi bối rối về cách thức hoạt động của sự chấp thuận ứng dụng](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Tôi không biết cách cấp quyền cho ứng dụng của mình](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Tôi không hiểu rõ sự khác biệt giữa quyền đại diện và quyền ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL) và API Graph Azure AD (AAD Graph)***

- Kể từ ngày 30 tháng 6 năm 2020, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Thư viện Xác thực Azure Active Directory (ADAL) và Azure AD Graph API (AAD Graph). Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.

- Bắt đầu từ ngày 30 tháng 6 năm 2022, chúng tôi sẽ kết thúc hỗ trợ cho ADAL và AAD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa. Do điều kiện này, dưới đây là các ngụ ý:

    - Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.

    - Các ứng dụng sử dụng AAD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối của AAD Graph sau

**Di chuyển ADAL**

Nếu bạn đang sử dụng các ứng dụng của Microsoft, chúng tôi khuyên bạn nên cập nhật lên Thư viện Xác thực Microsoft (MSAL), đây là thư viện có các tính năng và bản cập nhật bảo mật mới nhất. Đề xuất này nằm trong ngữ cảnh microsoft bắt đầu quy trình di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ. 

Việc di chuyển từ Microsoft từ các ứng dụng sang MSAL sẽ đảm bảo rằng các ứng dụng này được hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

1. [Đọc Câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Nếu bạn cần trợ giúp trong việc hiểu rõ ứng dụng nào sử dụng ADAL, chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng, đồng thời, nếu có, hãy liên hệ với bất kỳ nhà cung cấp phần mềm độc lập (ISV) hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.

**Di chuyển thiết Graph AAD**

Đối với các ứng dụng đang sử dụng AAD Graph, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng AAD Graph sang Microsoft Graph:

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. Cổng thông tin đăng ký ứng dụng Azure của bạn hiển thị các ứng dụng đang sử dụng AAD Graph. Chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng, đồng thời, nếu có, hãy liên hệ với bất kỳ nhà cung cấp phần mềm độc lập (ISV) hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn thông tin về mức sử Graph AAD trong đối tượng thuê của bạn.







