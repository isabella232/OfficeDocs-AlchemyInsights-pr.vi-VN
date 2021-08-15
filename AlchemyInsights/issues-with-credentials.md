---
title: Sự cố với thông tin xác thực
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986841"
---
# <a name="issues-with-credentials"></a>Sự cố với thông tin xác thực

Nền tảng định danh Microsoft và dòng thông tin xác thực máy khách [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) mô tả cách lập trình trực tiếp so với dòng cấp thông tin xác thực máy khách OAuth 2.0.

**Làm thế nào để tôi quản lý mật khẩu hoặc chứng chỉ của ứng dụng?**

Trong Azure CLI, bạn có thể sử dụng thông tin xác thực ứng dụng [az](https://docs.microsoft.com/cli/azure/ad/app/credential) để xóa, liệt kê hoặc đặt lại mật khẩu hoặc thông tin xác thực chứng chỉ của ứng dụng.

**Người dùng của tôi đặt lại mật khẩu như thế nào?**

Người dùng cần đăng [ký tự đặt lại mật khẩu trước](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) khi có thể đặt lại mật khẩu. Sau khi người dùng đã đăng ký, họ có thể làm theo hướng dẫn trong bài viết này để đặt lại mật khẩu: Đặt lại [mật khẩu cơ quan hoặc trường học của bạn.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Làm thế nào để người dùng của tôi thay đổi mật khẩu của họ?**

Người dùng có thể làm theo các bước trong bài viết này để thay đổi mật khẩu của họ: [Cách thay đổi mật khẩu của bạn.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Họ cũng có thể [Quản lý mật khẩu ứng dụng để xác minh hai bước.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Người dùng của tôi nhận được lỗi khi thay đổi hoặc đặt lại mật khẩu của họ**

Liên kết này sẽ cung cấp thông tin về các sự cố phổ biến có thể phát sinh khi người dùng cố gắng đặt lại mật khẩu: Các sự cố phổ biến [và các giải pháp của chúng](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Tôi đang gặp sự cố khi đặt lại mật khẩu người dùng**

- Hãy đảm bảo rằng bạn được phép đặt lại mật khẩu. *Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.

- Hãy đảm bảo rằng bạn hiểu các yêu cầu cấp phép:

  - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của mình:
    - **Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic
    - **Người dùng đám mây và/hoặc** người dùng tại chỗ - Azure AD Premium P1 hoặc P2, Enterprise Mobility + Security (EMS) hoặc Azure SECURE PRODUCTIVE ENTERPRISE (SPE)
    - Để tìm hiểu thêm về các yêu cầu cấp phép, hãy [xem mục Yêu cầu cấp phép cho đặt lại mật khẩu tự phục vụ Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Để đặt lại mật khẩu người dùng, hãy tìm người dùng trong Azure AD. Sau đó, trên lưỡi tổng quan cho người dùng đó, bấm vào nút "đặt lại mật khẩu".

**Nút đặt lại mật khẩu bị xám**

Bạn không được phép đặt lại **mật khẩu** của người dùng này. *Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.

**Tôi không thấy lưỡi đặt lại mật khẩu**

Bạn không được phép đặt lại mật khẩu. *Chỉ người quản trị toàn cục, mật khẩu và người dùng mới có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị có đặc quyền khác.

**Tôi không thấy lưỡi tích hợp tại chỗ trong tính năng đặt lại mật khẩu**

- Lưỡi tích hợp tại chỗ chỉ xuất hiện trong môi trường kết hợp - nghĩa là bạn đang sử dụng chức năng ghi lại mật khẩu để thao tác với mật khẩu người dùng tại chỗ.

- Bạn sẽ không thấy lưỡi này nếu:

  - Bạn đang không sử dụng chức năng ghi lại mật khẩu
  - Có sự cố với việc cài đặt/kết nối ghi lại mật khẩu của bạn
  - Đã xảy ra sự cố với việc cài đặt/kết nối Azure AD Kết nối
  - Để biết thêm các bước khắc phục sự cố ghi lại mật khẩu, hãy xem Khắc phục [sự cố ghi lại mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Tôi không biết cách đặt lại mật khẩu người dùng**

1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.
2. Đi đến **lưỡi Người dùng và nhóm,** chọn Tất **cả Người dùng**.
3. Chọn một người dùng từ danh sách.
4. Đối với người dùng đã chọn, chọn **Tổng** quan , rồi trong thanh lệnh, chọn Đặt **lại mật khẩu**.
5. Chọn nút **Đặt lại mật** khẩu và làm theo hướng dẫn trên màn hình.
    - Chỉ các thao tác đặt lại được thực hiện thông qua **cổng thông tin Azure hỗ** trợ ghi lại mật khẩu.

**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin Office 365 Admin hoặc ứng dụng Office 365 di động nhưng người dùng vẫn không thể đăng nhập**

Chức năng Ghi lại Mật khẩu không được hỗ trợ trong cổng thông tin này. Đặt lại mật khẩu người dùng trong cổng thông tin Azure.
