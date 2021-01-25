---
title: Các sự cố khi phát triển ứng dụng
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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974762"
---
# <a name="issues-developing-applications"></a>Các sự cố khi phát triển ứng dụng

Để khắc phục các sự cố phổ biến nhất khi tạo các ứng dụng Azure Active Directory (AD), hãy xem các bài viết sau đây:

- [Tôi gặp sự cố khi đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Tôi không biết cách thay đổi mã thông báo mặc định cho ứng dụng của tôi](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Tôi nhầm lẫn về cách thỏa thuận ứng dụng hoạt động](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Tôi không biết cách cấp quyền đối với ứng dụng của mình](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Tôi không hiểu sự khác biệt giữa quyền được ủy nhiệm và ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and AZURE AD GRAPH API (đồ họa Bad)** _

- Bắt đầu từ ngày 30 tháng 6, 2020, chúng tôi sẽ không còn thêm bất kỳ tính năng nào mới vào thư viện xác thực Azure Active Directory (ADAL) và Azure AD graph API (đồ họa Bad). Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.

- Bắt đầu từ ngày 30 tháng 6, 2022, chúng tôi sẽ kết thúc hỗ trợ đối với đồ thị ADAL và Bad và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật. Do điều kiện này, sau đây là các tác động:

    - Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào.

    - Các ứng dụng bằng cách sử dụng đồ thị Bad sau khi thời gian này không còn nhận được phản hồi từ điểm cuối của biểu đồ

*Di chuyển _ Adal**

Nếu bạn đang sử dụng ứng dụng Microsoft, chúng tôi khuyên bạn nên cập nhật lên thư viện xác thực Microsoft (MSAL), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất. Đề xuất này nằm trong ngữ cảnh của Microsoft bắt đầu quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối cùng hỗ trợ. 

Việc di chuyển theo Microsoft ứng dụng của nó vào MSAL đảm bảo rằng các ứng dụng sẽ lợi ích từ bảo mật và cải thiện tính năng của MSAL.

1. [Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Nếu bạn cần trợ giúp trong việc hiểu những ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn, nếu có, hãy đến bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.

**Di chuyển đồ thị trong Bad**

Đối với các ứng dụng đang sử dụng đồ thị Bad, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng đồ thị lên tiếng trên Microsoft graph:

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad. Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn thông tin về việc sử dụng đồ thị trong đối tượng thuê của bạn.







