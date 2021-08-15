---
title: Khắc phục sự cố Đăng nhập một lần cho Thiết bị Kết nối Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039268"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Khắc phục sự cố Đăng nhập một lần cho Thiết bị Kết nối Azure AD

Nếu bạn có môi trường Active Directory (AD) tại chỗ và bạn muốn liên kết các máy tính kết nối với miền AD với Azure AD, bạn có thể thực hiện việc này bằng cách thực hiện kết hợp Azure AD kết hợp. [Cách Thức: Lập kế hoạch triển khai Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) kết hợp sẽ cung cấp cho bạn các bước liên quan để triển khai kết hợp Azure AD kết hợp trong môi trường của bạn.

Để biết thêm thông tin, hãy xem mục Đặt cấu hình các thiết bị đã liên kết Azure AD cho Single-Sign Tại chỗ [để Windows Hello for Business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Các vấn đề về Mã thông báo Làm mới Chính (PRT)**

Mã thông báo Làm mới Chính (PRT) là một đối số quan trọng của xác thực Azure AD trên Windows 10, Windows Server 2016 trở lên, các thiết bị chạy iOS và Android. Đây là một Mã thông báo Web JSON (JWT) được cấp đặc biệt cho các nhà môi giới mã thông báo của bên thứ nhất của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị đó. Để biết chi tiết về cách phát hành, sử dụng và bảo vệ PRT trên các thiết Windows 10, hãy xem Mã thông báo Làm mới [Chính là gì?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES và AzureADPrt: YES**

Các trường này cho biết người dùng đã xác thực thành công với Azure AD khi đăng nhập vào thiết bị hay chưa. Nếu các giá trị **là NO**, thì đó có thể là do:

- Khóa lưu trữ bad trong TPM được liên kết với thiết bị khi đăng ký (chọn KeySignTest trong khi đang chạy mức cao)
- ID Đăng nhập Thay thế
- Không tìm thấy HTTP Proxy

Để khắc phục sự cố thiết bị bằng lệnh dsregcmd, hãy xem [Trạng thái SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
