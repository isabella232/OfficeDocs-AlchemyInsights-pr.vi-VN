---
title: Xóa kênh riêng của teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439909"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="11741-102">Xóa kênh riêng của teams</span><span class="sxs-lookup"><span data-stu-id="11741-102">Delete a Teams private channel</span></span>

<span data-ttu-id="11741-103">Microsoft đã biết sự cố xoá kênh riêng teams nếu bạn có chính sách lưu giữ SharePoint cho phép các trang web SharePoint cơ bản.</span><span class="sxs-lookup"><span data-stu-id="11741-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="11741-104">Microsoft đang làm việc khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="11741-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="11741-105">Trong khi đó, bạn có thể sử dụng giải pháp sau để xoá kênh riêng.</span><span class="sxs-lookup"><span data-stu-id="11741-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="11741-106">**Loại trừ bộ sưu tập nhóm/trang web khỏi chính sách lưu giữ SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="11741-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="11741-107">Đi tới cổng quản trị Office 365, và chọn **Hiển thị tất cả** trong ngăn điều hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="11741-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="11741-108">Trong **Trung tâm quản trị**, hãy truy cập chính sách ngăn ngừa mất dữ liệu **tuân thủ & bảo mật**  >  **Data Loss Prevention**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="11741-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="11741-109">Xác định bất kỳ chính sách áp dụng cho các trang web SharePoint và sửa đổi chính sách để các trang web SharePoint cho nhóm có kênh riêng không được bao gồm trong chính sách lưu giữ.</span><span class="sxs-lookup"><span data-stu-id="11741-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="11741-110">Lưu chính sách.</span><span class="sxs-lookup"><span data-stu-id="11741-110">Save the policy.</span></span>
    <span data-ttu-id="11741-111">Có thể mất đến 24 giờ để cài đặt chính sách có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="11741-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="11741-112">Sau khi trang web đã bị loại trừ, bạn có thể xóa kênh riêng tư.</span><span class="sxs-lookup"><span data-stu-id="11741-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="11741-113">Bạn ***có*** thể xóa kênh riêng bằng cách sử dụng Microsoft teams trên thiết bị Android của mình.</span><span class="sxs-lookup"><span data-stu-id="11741-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="11741-114">Thông tin SharePoint liên quan, xem [không thể xoá các mục trong SharePoint trực tuyến hoặc OneDrive dành cho doanh nghiệp](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="11741-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>