---
title: Password Writeback không hoạt động
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324945"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback không hoạt động

**Tôi đang gặp sự cố khi đặt cấu hình ghi lại mật khẩu**

- Ghi lại mật khẩu là một tính năng cao cấp.
- Hãy đảm bảo rằng bạn hiểu các yêu cầu cấp phép:
  - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của mình
  - **Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic
  - **Người dùng đám mây và/hoặc** người dùng tại chỗ - Azure AD Premium P1 hoặc P2, Enterprise Mobility + Security (EMS) hoặc Azure Secure Productive Enterprise AD (SPE)
    - Để tìm hiểu thêm về các yêu cầu cấp phép, hãy xem mục Yêu cầu cấp phép cho tính năng [đặt lại mật khẩu tự phục vụ của Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Bạn có ít nhất một tài khoản người quản trị và một tài khoản người dùng thử nghiệm có một trong các giấy phép thích hợp.
- Bạn phải kết nối Azure AD Kết nối trình mô phỏng Bộ kiểm soát miền chính để ghi lại mật khẩu có thể hoạt động. Bạn có thể đặt cấu hình Azure AD Kết nối sử  dụng Bộ điều khiển Miền Chính bằng cách bấm chuột phải vào các thuộc tính của bộ nối đồng bộ hóa Active Directory, rồi chọn đặt cấu hình phân **vùng thư mục.** Từ đó, hãy tìm phần thiết đặt **kết nối bộ điều khiển tên** miền và đánh dấu chọn hộp có tiêu đề chỉ sử dụng bộ điều khiển miền ưu **tiên.**
    **Lưu** ý :Nếu DC ưu tiên không phải là bộ mô phỏng PDC, Azure AD Kết nối sẽ vẫn liên hệ với PDC để ghi lại mật khẩu.
- Đặt lại mật khẩu đã được cấu hình và bật trong đối tượng thuê của bạn. Để biết thêm thông tin, hãy [xem mục Cho phép người dùng đặt lại mật khẩu Azure AD của họ.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Đảm bảo rằng tài khoản người quản trị đang được sử dụng để bật ghi lại mật khẩu là tài khoản người quản trị đám mây (được tạo trong Azure AD không phải AD tại chỗ)
- Bạn có một triển khai tại chỗ AD đơn hoặc nhiều rừng chạy Windows Server 2008 R2, Windows Server 2012 hoặc Windows Server 2012 R2 với cài đặt gói dịch vụ mới nhất
- Bạn đã cài đặt công cụ Kết nối Azure AD và bạn đã chuẩn bị môi trường AD để đồng bộ hóa với đám mây. Trước khi kiểm tra lại mật khẩu, hãy đảm bảo rằng trước tiên bạn phải hoàn thành quá trình nhập đầy đủ và đồng bộ đầy đủ từ cả AD và Azure AD trong Azure AD Kết nối.
- Để tìm hiểu thêm, hãy xem cách thực hiện đồng [bộ đầy đủ và nhập đầy đủ trong Azure AD Kết nối](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Tôi đang gặp sự cố với khả năng kết nối ghi lại mật khẩu**

1. Tải xuống và bật phiên bản mới [nhất của Azure AD Kết nối](https://www.microsoft.com/download/details.aspx?id=47594)
2. Cấu hình tường lửa: Công cụ Azure AD Kết nối (1.1.443 trở lên) sẽ cần truy nhập **HTTPS** bên ngoài để:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Cho phép duy trì kết nối không ở trạng thái liên tục trong ít nhất 2-3 phút

**Tôi vẫn gặp sự cố với việc ghi lại mật khẩu**

- Nếu bạn vẫn gặp khó khăn, hãy thử tắt và bật lại dịch vụ ghi lại mật khẩu trong công cụ Kết nối Azure AD
- Để tìm hiểu thêm, hãy xem cách [tắt và bật lại ghi lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
