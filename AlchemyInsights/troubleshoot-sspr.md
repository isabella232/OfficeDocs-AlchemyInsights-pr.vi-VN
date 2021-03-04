---
title: Khắc phục sự cố SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430360"
---
# <a name="troubleshoot-sspr"></a>Khắc phục sự cố SSPR

**Tôi đang gặp sự cố về cấu hình đặt lại mật khẩu**

- Nếu bạn là người quản trị và tìm cách bật tính năng đặt lại mật khẩu tự phục vụ, hãy xem [hướng dẫn bật SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), để cấu hình đặt lại mật khẩu cho tổ chức của bạn. Bạn cũng có thể muốn xem lại các [yêu cầu cấp phép](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn.
    - **Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC
    - Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)
- Để biết thêm thông tin về việc đặt lại mật khẩu tự phục vụ, hãy xem lại câu [hỏi thường gặp của chúng tôi](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tôi nhận được thông báo lỗi**

Xem lại bài viết này để tìm các lỗi thường gặp và giải pháp: [khắc phục sự cố đặt lại mật khẩu tự phục vụ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi đang gặp sự cố với chính sách đặt lại mật khẩu của tôi**

- Nếu chính sách đặt lại mật khẩu của bạn không phải là hành xử như mong muốn, hoặc nếu bạn có thắc mắc về chính sách đặt lại mật khẩu, hãy xem lại bài viết này: [chính sách mật khẩu và các hạn chế trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Các chính sách đặt lại mật khẩu không áp dụng cho người quản trị. Microsoft tham lực một chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho bất kỳ vai trò người quản trị Azure nào. Hãy đảm bảo rằng bạn đang thử nghiệm với người dùng không phải là người quản trị. Để biết thêm thông tin về chính sách đặt lại người quản trị, hãy xem bài viết này: [sự khác biệt về chính sách đặt lại người quản trị](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Tôi không muốn người dùng của mình đăng ký thông tin bảo mật bổ sung để đặt lại mật khẩu**

Bạn có thể có dữ liệu sẵn (email và thuộc tính điện thoại) cho người dùng của bạn bằng cách dùng API, PowerShell hoặc Azure AD Connect. Để tìm hiểu cách đọc:

- [Triển khai việc đặt lại mật khẩu mà không yêu cầu người dùng đăng ký](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Việc đặt lại mật khẩu, dữ liệu nào được sử dụng](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi muốn người dùng của mình đăng ký thông tin bảo mật bổ sung của họ để đặt lại mật khẩu**

1. Có người dùng của bạn đăng ký thông tin bảo mật của họ để đặt lại mật khẩu tự phục vụ bằng cách hướng họ đến [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Sau khi dữ liệu được nhập cho người dùng (bởi người dùng hoặc người quản trị), hãy hướng dẫn người dùng của bạn đến [aka.MS/sspr](https://passwordreset.microsoftonline.com/) để người dùng của bạn có thể được quyền đặt lại mật khẩu của riêng họ.
1. Nếu người dùng vẫn gặp vấn đề mà họ có **thể liên** kết hoặc **mật khẩu Hash** người dùng đồng bộ. Điều này có nghĩa là có vấn đề với dịch vụ Writeback mật khẩu.