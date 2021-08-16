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
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101984"
---
# <a name="device-writeback"></a>Device Writeback

Thiết bị Writeback được sử dụng trong các kịch bản sau đây:

- Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Bật Quyền truy nhập có Điều kiện dựa trên thiết bị được bảo vệ bằng ADFS (2012 R2 trở lên) (dựa vào tin tưởng của bên)

    > [!NOTE]
    > Cần có đăng ký Azure AD Premium để ghi lại thiết bị.

Điều này cung cấp bảo mật và đảm bảo bổ sung rằng quyền truy nhập vào các ứng dụng chỉ được cấp cho các thiết bị tin cậy. Để biết thêm thông tin [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) về Truy nhập có Điều kiện, hãy xem Quản lý Rủi ro với Truy nhập có Điều kiện và Thiết lập Truy nhập Có điều kiện tại cơ sở [bằng cách Azure Active Directory ký Thiết bị.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Để biết thêm thông tin về Bật ghi lại thiết bị cho thiết bị, hãy [xem Bật Ghi lại thiết bị](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
