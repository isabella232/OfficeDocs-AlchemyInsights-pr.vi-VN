---
title: Đọc Nhật ký kiểm tra cho các sự kiện đã xóa
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483323"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="39131-102">Đọc Nhật ký kiểm tra cho các sự kiện đã xóa</span><span class="sxs-lookup"><span data-stu-id="39131-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="39131-103">Sau đây là cách thực hiện:</span><span class="sxs-lookup"><span data-stu-id="39131-103">Here's how to do this:</span></span>

1. <span data-ttu-id="39131-104">Đi đến [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="39131-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="39131-105">Chọn **Tìm**  >  [**kiếm Nhật ký kiểm**](https://go.microsoft.com/fwlink/?linkid=2103759)tra.</span><span class="sxs-lookup"><span data-stu-id="39131-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="39131-106">Nếu bạn thấy thông báo rằng bạn cần bật tính năng này, hãy tiếp tục và bật trước.</span><span class="sxs-lookup"><span data-stu-id="39131-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="39131-107">Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể kéo dữ liệu từ ngày trước đó.</span><span class="sxs-lookup"><span data-stu-id="39131-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="39131-108">Chọn **hoạt động**, rồi tìm các **hoạt động của hộp thư Exchange**.</span><span class="sxs-lookup"><span data-stu-id="39131-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="39131-109">Chọn các **thư đã xóa khỏi thư mục các mục đã xóa** và đã **chuyển thư vào các** tùy chọn thư mục mục đã xóa.</span><span class="sxs-lookup"><span data-stu-id="39131-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="39131-110">Khi bạn đã thực hiện xong, hãy bấm vào bên ngoài ngăn để giảm thiểu ngăn **hoạt động** .</span><span class="sxs-lookup"><span data-stu-id="39131-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="39131-111">Xác định phạm vi ngày, sau đó trong hộp **người dùng** , hãy chọn tên người dùng cho người dùng mà bạn muốn điều tra.</span><span class="sxs-lookup"><span data-stu-id="39131-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="39131-112">Bạn có thể chọn nhiều người dùng cùng lúc.</span><span class="sxs-lookup"><span data-stu-id="39131-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="39131-113">Chọn **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="39131-113">Select **Search**.</span></span> <span data-ttu-id="39131-114">Các hoạt động sẽ xuất hiện bên dưới **kết quả**.</span><span class="sxs-lookup"><span data-stu-id="39131-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="39131-115">Để xem chi tiết, hãy chọn một hoạt động, rồi chọn **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="39131-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="39131-116">Thông tin bổ sung về mục đã xóa, chẳng hạn như dòng chủ đề và vị trí của mục khi thư đã bị xóa, được hiển thị trong trường **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="39131-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="39131-117">Bạn không thể khôi phục các mục đã xóa bằng tính năng Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="39131-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="39131-118">Để khôi phục các mục đã xóa, hãy xem [khôi phục các mục hoặc email đã xóa trong Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="39131-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="39131-119">Để tìm hiểu thêm, hãy xem [Tìm kiếm Nhật ký kiểm tra Office 365 để khắc phục các kịch bản phổ biến](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="39131-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
