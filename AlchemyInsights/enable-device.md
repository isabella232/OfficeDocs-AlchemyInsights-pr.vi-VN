---
title: Bật Thiết bị
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
- "8278"
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003515"
---
# <a name="enable-device"></a>Bật Thiết bị

**Để bật thiết bị bằng lệnh Powershell**

Chạy các lệnh sau đây:

- Để có được đối tượng của thiết bị: `Get-MsolDevice -Name <Name>`
- Để bật thiết bị: `Enable-MsolDevice -DeviceId <DeviceId>`

Để biết thêm thông tin về Cấu hình Kết hợp Kết hợp trên các tên miền được quản lý, hãy xem [Cấu hình Kết hợp Kết hợp.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
