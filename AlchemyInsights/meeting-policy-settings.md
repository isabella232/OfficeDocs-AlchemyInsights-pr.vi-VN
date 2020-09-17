---
title: Thiết đặt chính sách cuộc họp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794356"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6dfa2-102">Quản lý chính sách cuộc họp trong nhóm Microsoft</span><span class="sxs-lookup"><span data-stu-id="6dfa2-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6dfa2-103">**Lưu ý: có thể mất đến 24 giờ để thay đổi chính sách có hiệu lực đối với người dùng.**</span><span class="sxs-lookup"><span data-stu-id="6dfa2-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="6dfa2-104">Có thể bạn không thể thực hiện thay đổi đối với các chính sách mới được tạo ngay lập tức; Hãy chờ 4 giờ và cố gắng sửa đổi lại chính sách mới được tạo.</span><span class="sxs-lookup"><span data-stu-id="6dfa2-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="6dfa2-105">Các chính sách cuộc họp được dùng để điều khiển các tính năng sẵn dùng cho những người dự cuộc họp cho các cuộc họp được lên lịch bởi người dùng trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="6dfa2-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6dfa2-106">Một số tính năng của chính sách cuộc họp có thể không được thực hiện trong Trung tâm quản trị nhóm nào đó (đây là các tính năng có nhãn "Coming Soon" trong tài liệu).</span><span class="sxs-lookup"><span data-stu-id="6dfa2-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6dfa2-107">Trong trường hợp này, hoặc nếu bạn nhận được lỗi như "chúng tôi không thể cập nhật chính sách ngay bây giờ nhưng thử lại sau" trong Trung tâm quản trị nhóm Microsoft, chúng tôi khuyên bạn nên sử dụng PowerShell để tạo hoặc sửa đổi chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="6dfa2-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6dfa2-108">Để biết thêm thông tin về chính sách cuộc họp, hãy xem các tài nguyên sau đây:</span><span class="sxs-lookup"><span data-stu-id="6dfa2-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6dfa2-109">Để tìm hiểu về việc tạo chính sách, thực hiện thay đổi và gán người dùng vào chính sách, hãy xem [quản lý chính sách cuộc họp trong nhóm](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6dfa2-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6dfa2-110">Để thực hiện thay đổi chính sách bằng lệnh ghép ngắn PowerShell, hãy xem [tổng quan về các nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="6dfa2-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6dfa2-111">Bạn cần sử dụng [mô-đun của Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) cho các chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="6dfa2-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6dfa2-112">Xem lại [tài liệu ngắn lệnh ghép ngắn \*-csteamsmeetingđể](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="6dfa2-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

