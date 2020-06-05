---
title: Bắt đầu với sự kiện trực tiếp của teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 6ddb1e74d6c7217303da4f21a3bd71cdab3eb871
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563640"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="f1dc2-102">Bắt đầu với sự kiện trực tiếp của teams</span><span class="sxs-lookup"><span data-stu-id="f1dc2-102">Getting started with Teams live events</span></span>

<span data-ttu-id="f1dc2-103">Sự kiện trực tiếp của Microsoft teams là một phần mở rộng của các cuộc họp teams cho phép bạn lên lịch và tạo các sự kiện phát trực tuyến đến các đối tượng lớn trên mạng.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="f1dc2-104">Để tạo một sự kiện trực tiếp, bạn sẽ cần những việc sau:</span><span class="sxs-lookup"><span data-stu-id="f1dc2-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="f1dc2-105">Trước tiên, hãy xác nhận sự kiện teams Live có [ở quốc gia và khu vực của bạn](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Sự kiện trực tiếp chưa được hỗ trợ ở một số quốc gia.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="f1dc2-106">Nếu bạn đã gán giấy phép và đặt chính sách, nhưng vẫn không thể tạo sự kiện trực tiếp của teams, có thể bạn đang ở quốc gia hoặc khu vực mà sự kiện trực tiếp chưa khả dụng.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="f1dc2-107">Giấy phép [office 365 Enterprise E1, E3, hoặc E5 hoặc giấy phép office 365 A3 hoặc A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="f1dc2-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="f1dc2-108">**Lưu ý**: do sự gia tăng gần đây trong việc sử dụng các nhóm, khi bạn chỉ định giấy phép teams cho một người dùng, có thể mất khoảng 24 giờ trước khi chúng được thiết lập đầy đủ.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="f1dc2-109">Cho đến lúc đó, bạn sẽ không thể chỉ định chính sách teams cho họ và họ có thể không có quyền truy cập vào một số tính năng của teams như gọi điện và hội thảo âm thanh.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="f1dc2-110">Quyền [tạo sự kiện trực tiếp trong Trung tâm quản trị Microsoft teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="f1dc2-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="f1dc2-111">Quyền [tạo sự kiện trực tiếp trong Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (đối với các sự kiện được sản xuất bằng ứng dụng hoặc thiết bị phát sóng bên ngoài).</span><span class="sxs-lookup"><span data-stu-id="f1dc2-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="f1dc2-112">Thành viên nhóm đầy đủ trong org (không thể là khách hoặc từ tổ chức khác).</span><span class="sxs-lookup"><span data-stu-id="f1dc2-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="f1dc2-113">Lập lịch cuộc họp riêng, chia sẻ màn hình và chia sẻ video IP, đã bật trong chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="f1dc2-114">[Thực tiễn tốt nhất](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) cho các sự kiện trực tiếp teams.</span><span class="sxs-lookup"><span data-stu-id="f1dc2-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="f1dc2-115">Để biết thêm thông tin, vui lòng xem [bắt đầu với sự kiện trực tiếp của Microsoft teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="f1dc2-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>