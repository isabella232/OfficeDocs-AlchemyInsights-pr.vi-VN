---
title: Writeback mật khẩu không hoạt động
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243733"
---
# <a name="password-writeback-is-not-working"></a>Writeback mật khẩu không hoạt động

**Tôi đang gặp sự cố về cấu hình writeback mật khẩu**

- Trả về mật khẩu là một tính năng Premium.
- Hãy đảm bảo rằng bạn hiểu được các yêu cầu cấp phép:
  - Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn
  - **Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC
  - Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)
    - Để tìm hiểu thêm về các yêu cầu cấp phép, hãy xem mục [yêu cầu cấp phép cho AZURE AD self-đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Bạn có ít nhất một tài khoản người quản trị và một tài khoản người dùng kiểm tra với một trong số giấy phép thích hợp.
- Bạn phải kết nối Azure AD kết nối với trình giả lập bộ điều khiển tên miền chính để làm việc với mật khẩu. Bạn có thể cấu hình Azure AD Connect để dùng bộ điều khiển tên miền chính bằng cách bấm chuột phải vào **thuộc tính** của đường kết nối đồng bộ hóa Active Directory, sau đó chọn **cấu hình phân vùng thư mục**. Từ đó, hãy tìm phần **thiết đặt kết nối bộ điều khiển tên miền** và chọn hộp chỉ có tiêu đề dùng bộ kiểm **soát miền ưu tiên**.
  > [!NOTE]
  > Nếu các DC ưu tiên không phải là giả lập PDC, Azure AD Connect sẽ vẫn tiếp cận với PDC để bật lại mật khẩu.
- Đặt lại mật khẩu đã được cấu hình và được kích hoạt trong đối tượng thuê của bạn. Để biết thêm thông tin, hãy xem cho [phép người dùng đặt lại mật khẩu AZURE AD của họ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Hãy đảm bảo rằng tài khoản người quản trị đang được sử dụng để bật lại mật khẩu là tài khoản người quản trị đám mây (được tạo trong Azure AD không tại cơ sở tại chỗ)
- Bạn có triển khai tại cơ sở đơn hoặc nhiều rừng chạy Windows Server 2008 R2, Windows Server 2012 hoặc Windows Server 2012 R2 với các gói dịch vụ mới nhất được cài đặt
- Bạn đã cài đặt công cụ kết nối Azure AD và bạn đã chuẩn bị môi trường quảng cáo của mình để đồng bộ trên điện toán đám mây. Trước khi kiểm tra lại mật khẩu, hãy đảm bảo rằng trước tiên bạn hoàn thành nhập đầy đủ và đồng bộ đầy đủ từ cả quảng cáo và Azure AD trong Azure AD Connect.
- Để tìm hiểu thêm, hãy xem làm thế nào để thực hiện [đồng bộ đầy đủ và nhập đầy đủ trong AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Tôi đang gặp sự cố với kết nối writeback mật khẩu**

1. Tải xuống và bật Phiên bản mới nhất của [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Cấu hình tường lửa: công cụ Azure AD Connect (1.1.443 trở lên) sẽ cần truy nhập **https ra ngoài** vào:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Cho phép các kết nối nhàn rỗi tồn tại trong ít nhất 2-3 phút

**Tôi vẫn gặp sự cố với writeback mật khẩu**

- Nếu bạn vẫn gặp khó khăn, hãy thử tắt và bật lại dịch vụ trả về mật khẩu trong công cụ Azure AD Connect
- Để tìm hiểu thêm, hãy xem làm thế nào để [vô hiệu hóa và bật lại tính năng bật lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
