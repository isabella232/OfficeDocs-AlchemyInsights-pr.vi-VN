---
title: Khắc phục sự cố về SSPR
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038980"
---
# <a name="troubleshoot-sspr"></a>Khắc phục sự cố về SSPR

**Tôi đang gặp sự cố khi đặt cấu hình đặt lại mật khẩu**

- Nếu bạn là người quản trị và đang tìm cách bật tính năng tự đặt lại mật khẩu, hãy xem hướng dẫn cho phép [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), để đặt cấu hình đặt lại mật khẩu cho tổ chức của bạn. Bạn cũng có thể muốn xem lại các yêu [cầu cấp phép.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Bạn phải có ít nhất một giấy phép được gán trong tổ chức của mình.
    - **Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic
    - **Người dùng đám mây và/hoặc** người dùng tại chỗ - Azure AD Premium P1 hoặc P2, Enterprise Mobility + Security (EMS) hoặc Azure SECURE PRODUCTIVE ENTERPRISE (SPE)
- Để biết thêm câu hỏi về tính năng tự đặt lại mật khẩu, hãy xem lại Câu [hỏi thường gặp của chúng tôi.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi nhận được thông báo lỗi**

Xem lại bài viết này để tìm các lỗi thường gặp và giải pháp: Khắc phục [sự cố tự đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi đang gặp sự cố với chính sách đặt lại mật khẩu của mình**

- Nếu chính sách đặt lại mật khẩu của bạn không hoạt động như mong đợi hoặc nếu bạn có thắc mắc về chính sách đặt lại mật khẩu, hãy xem lại bài viết này: Chính sách mật khẩu và hạn chế [trong Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Chính sách đặt lại mật khẩu không áp dụng cho người quản trị. Microsoft sẽ thực thi chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho mọi vai trò người quản trị Azure. Đảm bảo rằng bạn đang thử nghiệm với người dùng không phải là người quản trị. Để biết thêm thông tin về chính sách đặt lại người quản trị, hãy xem bài viết sau: Sự [khác biệt về chính sách của người quản trị.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Tôi không muốn người dùng đăng ký thông tin bảo mật bổ sung cho việc đặt lại mật khẩu**

Bạn có thể nhập trước dữ liệu (thuộc tính email và điện thoại) cho người dùng của mình bằng cách sử dụng API, PowerShell hoặc Azure AD Kết nối. Để tìm hiểu cách đọc:

- [Triển khai đặt lại mật khẩu mà không yêu cầu người dùng đăng ký](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Dữ liệu nào được dùng bằng cách đặt lại mật khẩu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tôi muốn người dùng của tôi đăng ký thông tin bảo mật bổ sung cho việc đặt lại mật khẩu**

1. Yêu cầu người dùng đăng ký thông tin bảo mật của họ để tự đặt lại mật khẩu dịch vụ bằng cách hướng [họ aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Sau khi dữ liệu được cấp cho người dùng (bởi người dùng hoặc người quản trị), hãy hướng người dùng của bạn đến [aka.ms/sspr](https://passwordreset.microsoftonline.com/) để người dùng của bạn có thể được trao quyền đặt lại mật khẩu của riêng họ.
1. Nếu người dùng vẫn gặp sự cố, nhiều khả năng họ **là người dùng** được liên kết hoặc đồng bộ hóa bằng **mật** khẩu. Điều này có nghĩa là có thể có sự cố với dịch vụ Password Writeback.