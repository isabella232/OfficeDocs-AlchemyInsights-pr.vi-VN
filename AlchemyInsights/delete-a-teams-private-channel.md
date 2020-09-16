---
title: Xóa kênh riêng của nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730937"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="1c5d7-102">Xóa kênh riêng của nhóm</span><span class="sxs-lookup"><span data-stu-id="1c5d7-102">Delete a Teams private channel</span></span>

<span data-ttu-id="1c5d7-103">Microsoft đã biết về sự cố khi xóa một kênh riêng của nhóm nếu bạn đã bật các chính sách duy trì SharePoint cho site SharePoint cơ bản.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="1c5d7-104">Microsoft đang làm việc trên bản sửa lỗi.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="1c5d7-105">Trong lúc này, bạn có thể sử dụng các giải pháp thay thế sau đây để xóa kênh riêng tư.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="1c5d7-106">**Loại trừ nhóm/tuyển tập trang từ chính sách duy trì SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="1c5d7-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="1c5d7-107">Đi đến cổng thông tin quản trị Office 365, rồi chọn **Hiển thị tất cả** trong ngăn dẫn hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="1c5d7-108">Bên dưới **Trung tâm quản trị**, đi đến **bảo mật &**  >  chính sách**ngăn chặn dữ liệu**tuân thủ  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="1c5d7-109">Xác định bất kỳ chính sách nào áp dụng cho các site SharePoint và sửa đổi chính sách để trang SharePoint cho nhóm có chứa kênh riêng tư không được bao gồm trong chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="1c5d7-110">Lưu chính sách.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-110">Save the policy.</span></span>
    <span data-ttu-id="1c5d7-111">Có thể mất đến 24 giờ để thiết đặt chính sách có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="1c5d7-112">Sau khi site đã bị loại trừ, bạn có thể xóa kênh riêng tư.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="1c5d7-113">Bạn  ***có thể*** xóa kênh riêng tư bằng cách sử dụng Microsoft nhóm trên thiết bị Android của mình.</span><span class="sxs-lookup"><span data-stu-id="1c5d7-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="1c5d7-114">Để biết thông tin SharePoint liên quan, hãy xem [không thể xóa các mục trong SharePoint Online hoặc OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="1c5d7-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>