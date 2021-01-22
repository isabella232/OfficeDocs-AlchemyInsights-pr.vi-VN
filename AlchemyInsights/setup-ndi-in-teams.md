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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935198"
---
# <a name="turn-on-ndi-technology"></a>Bật công nghệ NDI

Công nghệ NDI yêu cầu hai bước được bật cho người dùng:

1. Người quản trị đối tượng thuê phải bật thuộc tính ' AllowNDIStreaming ' trong chính sách Csteamsmeeting.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Sau khi thay đổi này có dân cư, người dùng cuối phải bật công nghệ NDI® cho máy khách cụ thể của họ từ **thiết đặt > quyền**.

Để biết thêm thông tin, hãy xem [sử dụng công nghệ NDI trong nhóm Microsoft](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
