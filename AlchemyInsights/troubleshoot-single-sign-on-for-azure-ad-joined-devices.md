---
title: Khắc phục sự cố đăng nhập một lần cho Azure AD đã gia nhập thiết bị
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037338"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Khắc phục sự cố đăng nhập một lần cho Azure AD đã gia nhập thiết bị

Nếu bạn có môi trường Active Directory (AD) tại cơ sở và bạn muốn gia nhập vào các máy tính của bạn tham gia vào Azure AD, bạn có thể thực hiện điều này bằng cách kết hợp kết hợp Azure AD join. [Cách thức: lập kế hoạch cho việc thực hiện kết hợp Azure Active Directory của bạn](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sẽ cung cấp cho bạn các bước liên quan để thực hiện kết hợp Azure AD join trong môi trường của bạn.

Để biết thêm thông tin, hãy xem mục [đặt cấu hình AZURE AD đã gia nhập thiết bị cho các Single-Sign tại cơ sở khi sử dụng Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Các sự cố mã thông báo làm mới (PRT) chính**

Một mã thông báo làm mới chính (PRT) là một artifact chính của xác thực Azure AD trên Windows 10, Windows Server 2016 và các thiết bị chạy sau, iOS và Android. Đây là một mã thông báo web JSON (JWT) đặc biệt được phát hành cho môi giới mã thông báo đầu tiên của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị này. Để biết chi tiết về cách thức phát hành của PRT, được sử dụng và bảo vệ trên thiết bị chạy Windows 10, hãy xem mã thông báo [làm mới chính là gì?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: có và AzureADPrt: có**

Những trường này cho biết người dùng đã xác thực thành công để Azure AD khi đăng nhập vào thiết bị hay không. Nếu các giá trị là **không có**, có thể là do:

- Phím lưu trữ xấu trong TPM được liên kết với thiết bị sau khi đăng ký (kiểm tra kiểm tra phím trong khi đang chạy nâng cao)
- ID đăng nhập thay thế
- Không tìm thấy proxy HTTP

Để khắc phục các thiết bị bằng cách dùng lệnh dsregcmd, hãy xem [trạng thái SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
