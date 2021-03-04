---
title: Tìm sự kiện được thực hiện trên quy tắc hộp thư đến
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430311"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="41ddc-102">Tìm sự kiện được thực hiện trên quy tắc hộp thư đến</span><span class="sxs-lookup"><span data-stu-id="41ddc-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="41ddc-103">Khi quy tắc hộp thư đến được tạo, thay đổi hoặc xóa bỏ, các sự kiện được ghi lại trong Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="41ddc-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="41ddc-104">Sau đây là cách xem lại chúng:</span><span class="sxs-lookup"><span data-stu-id="41ddc-104">Here's how to review them:</span></span>

1. <span data-ttu-id="41ddc-105">Đi đến [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="41ddc-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="41ddc-106">Chọn tìm kiếm > tìm kiếm Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="41ddc-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="41ddc-107">Nếu bạn thấy thông báo rằng bạn cần bật kiểm định, hãy tiếp tục và bật tính năng này ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="41ddc-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="41ddc-108">Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể kéo dữ liệu từ ngày trước đó.</span><span class="sxs-lookup"><span data-stu-id="41ddc-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="41ddc-109">Chọn trường hoạt động và tìm các hoạt động của hộp thư Exchange, rồi chọn New-InboxRule tạo quy tắc hộp thư đến từ Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="41ddc-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="41ddc-110">Khi bạn đã thực hiện xong, hãy bấm vào bên ngoài ngăn để giảm thiểu ngăn hoạt động.</span><span class="sxs-lookup"><span data-stu-id="41ddc-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="41ddc-111">Xác định phạm vi ngày, sau đó trong trường người dùng, hãy chọn tên người dùng cho người dùng mà bạn muốn điều tra.</span><span class="sxs-lookup"><span data-stu-id="41ddc-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="41ddc-112">Bạn có thể chọn nhiều người dùng cùng lúc.</span><span class="sxs-lookup"><span data-stu-id="41ddc-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="41ddc-113">Chọn tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="41ddc-113">Select Search.</span></span> <span data-ttu-id="41ddc-114">Các hoạt động sẽ xuất hiện bên dưới kết quả.</span><span class="sxs-lookup"><span data-stu-id="41ddc-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="41ddc-115">Để xem chi tiết, hãy chọn một hoạt động, rồi chọn xem thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="41ddc-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="41ddc-116">Bên dưới mục tham số, bạn có thể nhìn thấy tên của quy tắc, bộ điều kiện và các hành động mà quy tắc đó sẽ mất.</span><span class="sxs-lookup"><span data-stu-id="41ddc-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="41ddc-117">Để tìm hiểu thêm, hãy xem tìm kiếm Nhật ký kiểm tra Office 365 để khắc phục các kịch bản phổ biến.</span><span class="sxs-lookup"><span data-stu-id="41ddc-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>