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
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="4dbcb-102">Bật công nghệ NDI</span><span class="sxs-lookup"><span data-stu-id="4dbcb-102">Turn on NDI technology</span></span>

<span data-ttu-id="4dbcb-103">Công nghệ NDI yêu cầu hai bước được bật cho người dùng:</span><span class="sxs-lookup"><span data-stu-id="4dbcb-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="4dbcb-104">Người quản trị đối tượng thuê phải bật thuộc tính ' AllowNDIStreaming ' trong chính sách Csteamsmeeting.</span><span class="sxs-lookup"><span data-stu-id="4dbcb-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="4dbcb-105">Sau khi thay đổi này có dân cư, người dùng cuối phải bật công nghệ NDI® cho máy khách cụ thể của họ từ **thiết đặt > quyền**.</span><span class="sxs-lookup"><span data-stu-id="4dbcb-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="4dbcb-106">Để biết thêm thông tin, hãy xem [sử dụng công nghệ NDI trong nhóm Microsoft](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="4dbcb-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
