---
title: Bắt đầu với các sự kiện nhóm trực tiếp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677301"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="abe7a-102">Bắt đầu với các sự kiện nhóm trực tiếp</span><span class="sxs-lookup"><span data-stu-id="abe7a-102">Getting started with Teams live events</span></span>

<span data-ttu-id="abe7a-103">Sự kiện Microsoft nhóm trực tiếp là một phần mở rộng của các cuộc họp nhóm cho phép bạn lên lịch và tạo ra các sự kiện cho người xem trực tuyến lớn.</span><span class="sxs-lookup"><span data-stu-id="abe7a-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="abe7a-104">Để tạo sự kiện trực tiếp, bạn sẽ cần những điều sau đây:</span><span class="sxs-lookup"><span data-stu-id="abe7a-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="abe7a-105">Trước tiên, hãy xác nhận rằng các sự kiện trực tiếp của nhóm có [sẵn tại quốc gia và khu vực của bạn](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Các sự kiện trực tiếp vẫn chưa được hỗ trợ ở một số quốc gia.</span><span class="sxs-lookup"><span data-stu-id="abe7a-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="abe7a-106">Nếu bạn đã gán giấy phép và đặt chính sách, nhưng vẫn không thể tạo sự kiện trực tiếp nhóm, có thể bạn đang ở trong quốc gia hoặc khu vực mà tại đó các sự kiện vẫn chưa sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="abe7a-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="abe7a-107">Một [office 365 Enterprise E1, E3 hoặc E5 License hoặc giấy phép office 365 A3 hoặc A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="abe7a-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="abe7a-108">**Lưu ý**: do tính năng gia tăng nhóm trong việc sử dụng gần đây, khi bạn gán giấy phép nhóm cho người dùng, có thể mất khoảng 24 giờ trước khi chúng được thiết lập đầy đủ.</span><span class="sxs-lookup"><span data-stu-id="abe7a-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="abe7a-109">Cho đến lúc đó, bạn sẽ không thể gán chính sách nhóm cho họ và họ có thể không có quyền truy nhập vào một số tính năng nhóm như gọi và hội thảo âm thanh.</span><span class="sxs-lookup"><span data-stu-id="abe7a-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="abe7a-110">Quyền [tạo sự kiện trực tiếp trong Trung tâm quản trị nhóm Microsoft](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="abe7a-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="abe7a-111">Quyền [tạo sự kiện trực tiếp trong Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (cho các sự kiện được tạo bằng cách sử dụng một ứng dụng hoặc thiết bị phát rộng bên ngoài).</span><span class="sxs-lookup"><span data-stu-id="abe7a-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="abe7a-112">Thành viên nhóm đầy đủ trong tổ chức (không thể là khách mời hoặc từ tổ chức khác).</span><span class="sxs-lookup"><span data-stu-id="abe7a-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="abe7a-113">Lập lịch cuộc họp riêng tư, chia sẻ screenvà chia sẻ video IP, được bật trong chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="abe7a-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="abe7a-114">Cách [thực hành tốt nhất](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) cho các sự kiện trực tiếp của nhóm.</span><span class="sxs-lookup"><span data-stu-id="abe7a-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="abe7a-115">Để biết thêm thông tin, vui lòng xem mục [bắt đầu với các sự kiện Microsoft nhóm trực tiếp](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="abe7a-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>