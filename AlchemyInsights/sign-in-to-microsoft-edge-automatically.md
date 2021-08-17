---
title: Đăng nhập vào Microsoft Edge động
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050716"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Đăng nhập vào Microsoft Edge động

Microsoft Edge dùng tài khoản mặc định HĐH để tự động đăng nhập người dùng theo cách cấu hình thiết bị của người dùng. 

Kịch bản của mỗi kiểu cấu hình thiết bị và quy trình đăng nhập người dùng phụ thuộc của thiết bị được mô tả dưới đây:

- **Thiết bị là kết hợp/AAD-J:** Tùy chọn này sẵn dùng trên các Windows 10, bản cập nhật mức Windows và các phiên bản máy chủ tương ứng. Người dùng được tự động đăng nhập bằng tài khoản Azure Active Directory mình (AD).
- **Thiết bị kết nối theo miền**: Tùy chọn này sẵn dùng trên các Windows 10, bản cập nhật mức Windows và các phiên bản máy chủ tương ứng. Theo mặc định, người dùng có tài khoản tên miền không được đăng nhập tự động; để bật đăng nhập tự động cho họ, hãy sử dụng **chính sách ConfigureOnPremisesAccountAutoSignIn.** Để cho phép đăng nhập tự động cho người dùng có tài khoản Azure AD, hãy cân nhắc kết hợp các thiết bị của họ.
- Tài khoản mặc định của HĐH là tài khoản **Microsoft:** Tùy chọn này sẵn dùng trên Windows 10 RS3 (phiên bản 1709, bản dựng 10.0.16299) và các phiên bản mới hơn. Kịch bản không thể xảy ra trên các thiết bị doanh nghiệp. Tuy nhiên, nếu tài khoản HĐH mặc định là tài khoản Microsoft thì Microsoft Edge sẽ tự động đăng nhập người dùng bằng tài khoản Microsoft.
 
 
