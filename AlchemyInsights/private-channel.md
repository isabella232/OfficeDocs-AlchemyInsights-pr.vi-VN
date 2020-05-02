---
title: Kênh riêng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005460"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="fbc4c-102">Kênh riêng tư trong Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="fbc4c-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="fbc4c-103">Các kênh riêng tư là một tính năng mới trong Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="fbc4c-104">Lưu ý rằng các kênh riêng tư không thể chuyển đổi từ các kênh tiêu chuẩn hoặc ngược lại.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="fbc4c-105">Để biết chi tiết về các kênh riêng tư, chẳng hạn như thông tin về [việc tạo kênh riêng và](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [các trang web SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)riêng tư và kênh tư nhân, xem [các kênh riêng tư trong Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="fbc4c-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="fbc4c-106">**Lưu ý:** Vì cấu hình để lưu giữ các thư riêng tư không được hỗ trợ, người thuê với chính sách lưu giữ cho phép sẽ không có kênh riêng được kích hoạt theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="fbc4c-107">Bạn có thể bật các kênh riêng tư trong Trung tâm quản trị teams.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="fbc4c-108">Ngoài ra, lưu ý rằng mặc dù không hỗ trợ lưu trữ các tin nhắn kênh riêng tư, việc lưu giữ các tệp được chia sẻ trong các kênh riêng tư có hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="fbc4c-109">**Bạn cần một chủ sở hữu nhóm mới?**</span><span class="sxs-lookup"><span data-stu-id="fbc4c-109">**Need a new team owner?**</span></span>

<span data-ttu-id="fbc4c-110">Nếu chủ sở hữu kênh riêng của bạn rời khỏi, bạn có thể thêm chủ sở hữu nhóm mới qua teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="fbc4c-111">Truy cập vào [đây](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) để cài đặt đội PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="fbc4c-112">Đây là lệnh bạn sẽ cần:</span><span class="sxs-lookup"><span data-stu-id="fbc4c-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="fbc4c-113">Để biết thêm thông tin về teams PowerShell, xem [tổng quan về nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="fbc4c-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
