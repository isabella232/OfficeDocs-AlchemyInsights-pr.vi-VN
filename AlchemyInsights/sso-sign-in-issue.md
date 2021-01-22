---
title: Các vấn đề đăng nhập của người dùng SSO liền mạch
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935218"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Các vấn đề đăng nhập của người dùng SSO liền mạch

Sau khi người dùng được xác thực, trình duyệt sẽ lưu bộ đệm ẩn chứng danh của người dùng, để trên cùng một trình duyệt, ứng dụng sẽ tự động đăng nhập bằng cùng một tài khoản. Điều này có thể gây khó khăn cho người dùng khác hoặc một người dùng duy nhất để đăng nhập vào nhiều tài khoản trên một thiết bị. Để giải quyết vấn đề này: 1. Thử đăng nhập trên một trình duyệt khác. 4. Xóa bộ đệm ẩn của trình duyệt và/hoặc cookie và thử đăng nhập lại.

Nếu bạn vẫn gặp sự cố đăng nhập, chúng tôi khuyên bạn nên sau đây để chẩn đoán và tự động hóa các bước giải quyết:

1. Cài đặt [phần mở rộng của trình duyệt bảo mật ứng dụng của tôi](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) để giúp Azure Active Directory (Azure AD) để cung cấp chẩn đoán và giải pháp tốt hơn khi sử dụng trải nghiệm thử nghiệm trong cổng thông tin Azure.
2. Tái tạo lỗi bằng trải nghiệm thử nghiệm trong trang cấu hình ứng dụng trong cổng thông tin Azure. Để tìm hiểu thêm, hãy xem mục [các ứng dụng đăng nhập trên máy đơn của gỡ lỗi SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Nếu bạn sử dụng trải nghiệm thử nghiệm trong cổng thông tin Azure với phần mở rộng của trình duyệt bảo mật ứng dụng của tôi, bạn có thể **bỏ qua bước 4**.
4. Để mở trang cấu hình đăng nhập đơn trên SAML:
    - Mở [cổng thông tin Azure](https://portal.azure.com/) và đăng nhập với tư cách là **người quản trị toàn cầu hoặc người quản** trị **coadmin**.
    - Mở **phần mở rộng Azure Active Directory** bằng cách chọn **tất cả các dịch vụ** ở phía trên cùng của menu dẫn hướng bên trái chính.
    - Nhập "Azure Active Directory" trong hộp tìm kiếm bộ lọc và chọn mục **Azure Active Directory** .
    - Chọn các **ứng dụng doanh nghiệp** từ menu dẫn hướng bên trái của Azure Active Directory.
    - Chọn **tất cả các ứng dụng** để xem danh sách tất cả các ứng dụng của bạn. Nếu bạn không nhìn thấy ứng dụng mà bạn muốn hiển thị ở đây, hãy dùng điều khiển **bộ lọc** ở đầu **danh sách tất cả ứng dụng** và đặt tùy chọn **Hiển thị** cho **tất cả các ứng dụng**.
    - Chọn ứng dụng bạn muốn cấu hình cho đăng nhập đơn.
    - Sau khi tải ứng dụng, hãy chọn **đăng nhập đơn** từ menu dẫn hướng bên trái của ứng dụng.
    - Chọn **SSO dựa trên SAML**.
5. Dựa trên lỗi, để tìm hiểu thêm về các bước được đề xuất để theo dõi, hãy xem mục các [vấn đề đăng nhập vào các ứng dụng được đặt cấu hình đăng nhập vào SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Để khắc phục sự cố đăng nhập người dùng khác, hãy tham khảo hướng dẫn sau đây:
    - [Giao thức Sign-On đơn nhất](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Cách thức: khắc phục lỗi đăng nhập bằng cách sử dụng báo cáo Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Lời nhắc đồng ý không mong muốn](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Lỗi người dùng chấp thuận](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Các sự cố khi đăng nhập từ ứng dụng của tôi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Lỗi trên trang đăng nhập ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Sự cố khi đăng nhập vào ứng dụng Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
