---
title: Device Writeback
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
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320108"
---
# <a name="device-writeback"></a>Device Writeback

Thiết bị Writeback được sử dụng trong các kịch bản sau đây:

- Bật Kiểm [Windows Hello cho Doanh nghiệp bằng cách dùng triển khai tin cậy chứng chỉ hỗn hợp](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Bật Quyền truy nhập có Điều kiện dựa trên thiết bị được bảo vệ bằng ADFS (2012 R2 trở lên) (dựa vào tin tưởng của bên)

    **Lưu** ý : Bắt buộc phải có đăng ký Azure AD Premium để ghi lại thiết bị.

Điều này cung cấp bảo mật và đảm bảo bổ sung rằng quyền truy nhập vào các ứng dụng chỉ được cấp cho các thiết bị tin cậy. Để biết thêm thông tin [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) về Truy nhập có Điều kiện, hãy xem Quản lý Rủi ro với Truy nhập có Điều kiện và Thiết lập Truy nhập Có điều kiện tại cơ sở [bằng cách Azure Active Directory ký Thiết bị](https://docs.microsoft.com/azure/active-directory/devices/overview).

Để biết thêm thông tin về Bật ghi lại thiết bị cho thiết bị, hãy [xem Bật Ghi lại thiết bị](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
