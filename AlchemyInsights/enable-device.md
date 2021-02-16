---
title: Bật thiết bị
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
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256990"
---
# <a name="enable-device"></a>Bật thiết bị

**Để bật thiết bị bằng cách dùng lệnh PowerShell**

Chạy các lệnh sau đây:

- Để lấy đối tượng thiết bị: `Get-MsolDevice -Name <Name>`
- Để cho phép thiết bị: `Enable-MsolDevice -DeviceId <DeviceId>`

Để biết thêm thông tin về cách cấu hình kết hợp kết hợp trên tên miền được quản lý, hãy xem [cấu hình kết hợp gia nhập](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
