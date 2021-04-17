---
title: Cách bật SSO liền mạch
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825753"
---
# <a name="how-to-enable-seamless-sso"></a>Cách bật SSO liền mạch

Cho phép SSO liền mạch thông qua [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Nếu bạn đang thực hiện một bản cài đặt mới của Azure AD Connect, hãy chọn [đường dẫn cài đặt tùy chỉnh](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Tại trang **đăng nhập người dùng** , hãy chọn tùy chọn **bật đăng nhập đơn** .
  
Để xác nhận rằng bạn đã bật chính xác SSO đúng cách:
  
1. Đăng nhập vào [Trung tâm quản trị Azure Active Directory](https://aad.portal.azure.com) với tư cách là người quản trị toàn cầu.

2. Chọn **Azure Active Directory** trong ngăn bên trái.

3. Xác nhận đăng nhập đơn seamless được **bật**.

Để tìm hiểu thêm, hãy xem [Azure Active Directory liền mạch Single đăng nhập: bắt đầu nhanh](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  