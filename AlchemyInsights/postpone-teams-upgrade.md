---
title: Trì hoãn nâng cấp nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801253"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="b722c-102">Cách trì hoãn việc nâng cấp nhóm Microsoft-driven</span><span class="sxs-lookup"><span data-stu-id="b722c-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="b722c-103">**Quan trọng**: chúng tôi có thể giúp khắc phục sự cố này cho bạn bằng cách sử dụng chẩn đoán hỗ trợ, nhưng có vẻ như bạn đang không sử dụng trung tâm quản trị mới.</span><span class="sxs-lookup"><span data-stu-id="b722c-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="b722c-104">Để sử dụng trung tâm quản trị mới, hãy trượt các nút bật tắt ở phía trên cùng bên phải cho biết **Trung tâm quản trị mới** sang phải.</span><span class="sxs-lookup"><span data-stu-id="b722c-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="b722c-105">Sử dụng trung tâm quản trị mới, bấm vào mục **cần trợ giúp?** widget, nhập "hoãn nâng cấp nhóm", rồi làm theo các lời nhắc để chạy chẩn đoán.</span><span class="sxs-lookup"><span data-stu-id="b722c-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="b722c-106">Nếu bạn nhận được thông tin về việc nâng cấp tự động Microsoft-driven từ Skype for Business sang Microsoft nhóm và bạn muốn trì hoãn việc nâng cấp tự động vào một ngày sau đó, người quản trị toàn cầu của bạn có thể đăng nhập vào [cổng thông tin quản trị nhóm](https://admin.teams.microsoft.com/dashboard) và sau khi chọn nút **trạng thái làm mới** bên dưới nâng cấp Microsoft nhóm, hãy chọn nút trì **hoãn** .</span><span class="sxs-lookup"><span data-stu-id="b722c-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="b722c-107">Để xem ngày mới cho việc nâng cấp tự động của đối tượng thuê cho Microsoft nhóm, làm mới trang cổng thông tin quản trị nhóm.</span><span class="sxs-lookup"><span data-stu-id="b722c-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="b722c-108">**Lưu ý:** Nút trì **hoãn** sẽ chỉ sẵn dùng nếu bạn đã nhận được thông báo Trung tâm thông báo liên quan đến việc nâng cấp tự động.</span><span class="sxs-lookup"><span data-stu-id="b722c-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="b722c-109">Người quản trị toàn cầu cũng có thể chạy [Get-Cisteamsupgradestatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) để tìm hiểu thêm về trạng thái nâng cấp hiện tại của họ.</span><span class="sxs-lookup"><span data-stu-id="b722c-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
