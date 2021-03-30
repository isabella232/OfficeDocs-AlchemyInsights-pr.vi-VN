---
title: Single-Sign cho Azure Active Directory đã tham gia thiết bị
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405666"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Đăng nhập một lần cho Azure Active Directory đã tham gia thiết bị

Nếu bạn có môi trường Active Directory (AD) tại cơ sở và bạn muốn gia nhập vào các máy tính của bạn tham gia vào Azure AD, bạn có thể thực hiện điều này bằng cách kết hợp kết hợp Azure AD join. [Cách thức: lập kế hoạch cho việc thực hiện kết hợp Azure Active Directory của bạn](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sẽ cung cấp cho bạn các bước liên quan để thực hiện kết hợp Azure AD join trong môi trường của bạn.

[Cấu hình Azure AD đã tham gia các thiết bị cho Single-Sign tại cơ sở khi sử dụng Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

Các sự **cố mã thông báo làm mới (PRT) chính** Một mã thông báo làm mới chính (PRT) là một artifact chính của xác thực Azure AD trên Windows 10, Windows Server 2016 và các thiết bị chạy sau, iOS và Android. Đây là một mã thông báo web JSON (JWT) đặc biệt được phát hành cho môi giới mã thông báo đầu tiên của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị này. [Trong mã bản làm mới chính là gì?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), chúng tôi sẽ cung cấp chi tiết về cách thức phát hành của PRT, được sử dụng và bảo vệ trên các thiết bị chạy Windows 10.

**Wamdefaultset: có và AzureADPrt: có** Những trường này cho biết người dùng đã xác thực thành công để Azure AD khi đăng nhập vào thiết bị hay không. Nếu các giá trị là **không có**, thì có thể là do:

- Phím lưu trữ xấu trong TPM được liên kết với thiết bị sau khi đăng ký (kiểm tra kiểm tra phím trong khi đang chạy nâng cao).
- ID đăng nhập thay thế
- Không tìm thấy proxy HTTP

Khắc phục sự cố các thiết bị sử dụng lệnh dsregcmd- [SSO State](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
