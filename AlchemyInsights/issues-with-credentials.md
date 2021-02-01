---
title: Các vấn đề với chứng danh
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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063724"
---
# <a name="issues-with-credentials"></a>Các vấn đề với chứng danh

[Nền tảng Microsoft Identity và dòng chứng danh máy khách oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) mô tả cách chương trình trực tiếp chống lại chứng danh máy khách của oauth 2,0.

**Làm thế nào để tôi quản lý mật khẩu của ứng dụng hoặc chứng danh chứng chỉ?**

Trong Azure CLI, bạn có thể sử dụng thông tin xác thực [ứng dụng AZ AD](https://docs.microsoft.com/cli/azure/ad/app/credential) để xóa, danh sách hoặc đặt lại mật khẩu hoặc chứng danh chứng chỉ của ứng dụng.

**Làm thế nào để người dùng của tôi đặt lại mật khẩu?**

Người dùng cần [đăng ký để đặt lại mật khẩu tự phục vụ](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) trước khi họ có thể đặt lại mật khẩu của họ. Sau khi người dùng đã đăng ký, họ có thể làm theo các hướng dẫn trong bài viết này để đặt lại mật khẩu của họ: [đặt lại mật khẩu cơ quan hoặc trường học của bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Người dùng của tôi thay đổi mật khẩu của mình như thế nào?**

Người dùng có thể làm theo các bước trong bài viết này để thay đổi mật khẩu của họ: [cách thay đổi mật khẩu của bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Họ cũng có thể [quản lý mật khẩu ứng dụng để xác minh hai bước](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Người dùng của tôi đang nhận được lỗi khi thay đổi hoặc đặt lại mật khẩu của họ**

Liên kết này sẽ cung cấp thông tin về các sự cố phổ biến có thể phát sinh khi người dùng đang tìm cách đặt lại mật khẩu: các [vấn đề thường gặp và giải pháp của họ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Tôi đang gặp sự cố khi đặt lại mật khẩu của người dùng**

- Hãy đảm bảo rằng bạn được ủy quyền để đặt lại mật khẩu. *Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.

- Hãy đảm bảo bạn hiểu được các yêu cầu cấp phép:

  - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn:
    - **Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC
    - Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)
    - Để tìm hiểu thêm về các yêu cầu cấp phép, hãy xem các [yêu cầu cấp phép cho AZURE AD tự đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Để đặt lại mật khẩu người dùng, hãy tìm người dùng trong Azure AD. Sau đó, trên lưỡi tổng quan cho người dùng đó, hãy bấm vào nút "đặt lại mật khẩu".

**Nút đặt lại mật khẩu bị mờ đi**

Bạn không được phép đặt lại mật khẩu của người dùng **này** . *Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.

**Tôi không nhìn thấy lưỡi đặt lại mật khẩu**

Bạn không được phép đặt lại mật khẩu. *Chỉ có người quản trị toàn cầu, mật khẩu và người dùng có thể đặt lại mật khẩu người dùng.* Người quản trị toàn cầu cũng có thể đặt lại mật khẩu của người quản trị đặc quyền khác.

**Tôi không nhìn thấy lưỡi kiếm tích hợp tại cơ sở trong đặt lại mật khẩu**

- Lưỡi tích hợp tại cơ sở chỉ xuất hiện trong môi trường hỗn hợp-nghĩa là bạn đang sử dụng writeback để thao tác mật khẩu của người dùng tại cơ sở.

- Bạn không thấy lưỡi này nếu:

  - Bạn không sử dụng writeback mật khẩu
  - Có vấn đề với việc cài đặt/kết nối của writeback mật khẩu
  - Có vấn đề với việc cài đặt/kết nối của Azure AD Connect
  - Để biết thêm các bước khắc phục sự cố với mật khẩu trở lại, hãy xem [khắc phục sự cố writeback mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Tôi không biết làm thế nào để đặt lại mật khẩu người dùng**

1. Đăng nhập vào cổng thông tin Azure với tư cách là người quản trị thích hợp.
2. Đi đến lưỡi **người dùng và nhóm** , chọn **tất cả người dùng**.
3. Chọn một người dùng từ danh sách.
4. Đối với người dùng đã chọn, hãy chọn **tổng quan**, rồi trong thanh lệnh, chọn **đặt lại mật khẩu**.
5. Chọn nút **đặt lại mật khẩu** và làm theo hướng dẫn trên màn hình.
    - Chỉ Reset được thực hiện thông qua dịch vụ hỗ trợ **Azure Portal** .

**Tôi đặt lại mật khẩu người dùng tại cơ sở từ cổng thông tin quản trị Office 365 hoặc ứng dụng Office 365 dành cho thiết bị di động nhưng người dùng vẫn không thể đăng nhập**

Không hỗ trợ mật khẩu của Writeback trong cổng thông tin này. Đặt lại mật khẩu người dùng một lần nữa trong cổng thông tin Azure.
