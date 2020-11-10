---
title: Sử dụng Giphys trong các cuộc hội thoại Nhóm
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982572"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="f5a71-102">Sử dụng Giphys trong các cuộc hội thoại Nhóm</span><span class="sxs-lookup"><span data-stu-id="f5a71-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="f5a71-103">Truy nhập giphys trong nhóm trò chuyện được bật theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="f5a71-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="f5a71-104">Với tư cách là người quản trị, bạn có thể kiểm soát nếu Giphys sẵn có cho người dùng bằng [cách đặt chính sách gửi tin nhắn](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) và đảm bảo rằng **việc sử dụng giphys trong các cuộc hội thoại** đang **bật**.</span><span class="sxs-lookup"><span data-stu-id="f5a71-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="f5a71-105">Nếu GIFs không hoạt động như dự kiến trong các cuộc hội thoại nhóm, hãy xác nhận:</span><span class="sxs-lookup"><span data-stu-id="f5a71-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="f5a71-106">[Chính sách nhắn tin](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) cần để cho phép Giphys.</span><span class="sxs-lookup"><span data-stu-id="f5a71-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="f5a71-107">Để xác nhận bằng cách sử dụng lệnh ghép ngắn PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f5a71-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="f5a71-108">Xác nhận rằng bạn có thể [quản lý các nhóm bằng PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="f5a71-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="f5a71-109">Chạy lệnh PowerShell [Get-Cisteamsmessagingpolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) và xác minh rằng **allowgiphy** được đặt là **True**.</span><span class="sxs-lookup"><span data-stu-id="f5a71-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="f5a71-110">Nếu **Allowgiphy** được đặt là **false** , hãy chạy lệnh PowerShell sau đây là lệnh [-Xsteamsmessagingpolicy-Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="f5a71-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="f5a71-111">[Những trải nghiệm kết nối tùy chọn](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) cần được kích hoạt để cho phép truy nhập vào URL của giphy.</span><span class="sxs-lookup"><span data-stu-id="f5a71-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="f5a71-112">Nếu bạn có nhiều chính sách nhắn tin theo nhóm được cấu hình cho đối tượng thuê của mình, bạn có thể xác định danh tính của chính sách được gán cho người dùng bị ảnh hưởng bằng lệnh PowerShell [Get-Xsonlineuser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Chọn TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="f5a71-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
