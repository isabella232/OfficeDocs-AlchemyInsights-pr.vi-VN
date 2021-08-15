---
title: Bật công nghệ NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023544"
---
# <a name="turn-on-ndi-technology"></a>Bật công nghệ NDI

Công nghệ NDI yêu cầu phải bật hai bước cho người dùng:

1. Người quản trị đối tượng thuê phải bật thuộc tính 'AllowNDIStreaming' trong CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Sau khi thay đổi này đã được thực hiện, người dùng cuối phải bật công nghệ NDI® cho máy khách cụ thể của Cài đặt > **quyền.**

Để biết thêm thông tin, [hãy xem mục Sử dụng công nghệ NDI trong Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
