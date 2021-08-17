---
title: Single-Sign bật cho các thiết Azure Active Directory nối
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050032"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Đăng nhập một lần cho Thiết Azure Active Directory Nối

Nếu bạn có môi trường Active Directory (AD) tại chỗ và bạn muốn liên kết các máy tính kết nối với miền AD với Azure AD, bạn có thể thực hiện việc này bằng cách thực hiện kết hợp Azure AD kết hợp. [Cách Thức: Lập kế hoạch triển khai Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) kết hợp sẽ cung cấp cho bạn các bước liên quan để triển khai kết hợp Azure AD kết hợp trong môi trường của bạn.

[Đặt cấu hình các thiết bị đã kết hợp Azure AD cho Single-Sign tại chỗ Đang sử dụng Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Các vấn đề về Mã thông báo Làm mới Chính (PRT)** Mã thông báo Làm mới Chính (PRT) là một đối số quan trọng của xác thực Azure AD trên Windows 10, Windows Server 2016 trở lên, các thiết bị chạy iOS và Android. Đây là một Mã thông báo Web JSON (JWT) được cấp đặc biệt cho các nhà môi giới mã thông báo của bên thứ nhất của Microsoft để cho phép đăng nhập một lần (SSO) trên các ứng dụng được sử dụng trên các thiết bị đó. Trong Mã thông báo Làm mới Chính là [gì?,](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)chúng tôi sẽ cung cấp chi tiết về cách phát hành, sử dụng và bảo vệ PRT trên các Windows 10 của bạn.

**WamDefaultSet: YES và AzureADPrt: YES** Các trường này cho biết người dùng đã xác thực thành công với Azure AD khi đăng nhập vào thiết bị hay chưa. Nếu các giá trị là **NO** thì có thể là do:

- Khóa lưu trữ bad trong TPM được liên kết với thiết bị khi đăng ký (chọn KeySignTest trong khi chạy mức cao).
- ID Đăng nhập Thay thế
- Không tìm thấy HTTP Proxy

Khắc phục sự cố thiết bị bằng lệnh dsregcmd - [Trạng thái SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
