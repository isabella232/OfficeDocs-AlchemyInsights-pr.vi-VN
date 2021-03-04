---
title: Tìm hiểu xem ai đã thiết lập chuyển tiếp trên hộp thư và cách thức
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430305"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="8c723-102">Tìm hiểu xem ai đã thiết lập chuyển tiếp trên hộp thư và cách thức</span><span class="sxs-lookup"><span data-stu-id="8c723-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="8c723-103">Nếu việc chuyển tiếp bên ngoài được đặt trên một hộp thư, hoạt động được kiểm toán như là một phần của lệnh ghép ngắn Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="8c723-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="8c723-104">Sau đây là cách tìm kiếm hoạt động trong Nhật ký kiểm tra:</span><span class="sxs-lookup"><span data-stu-id="8c723-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="8c723-105">Đi đến [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="8c723-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="8c723-106">Chọn **Tìm** >  **kiếm Nhật ký kiểm** tra.</span><span class="sxs-lookup"><span data-stu-id="8c723-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="8c723-107">Nếu bạn thấy thông báo rằng bạn cần bật kiểm định, hãy tiếp tục và bật tính năng này ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="8c723-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="8c723-108">Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể kéo dữ liệu từ ngày trước đó.</span><span class="sxs-lookup"><span data-stu-id="8c723-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="8c723-109">Đảm bảo rằng trường **hoạt động** được thiết lập để **Hiển thị kết quả cho tất cả các hoạt động** (mặc định).</span><span class="sxs-lookup"><span data-stu-id="8c723-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="8c723-110">Xác định phạm vi ngày.</span><span class="sxs-lookup"><span data-stu-id="8c723-110">Specify the date range.</span></span> <span data-ttu-id="8c723-111">Bạn không cần phải xác định tên người dùng.</span><span class="sxs-lookup"><span data-stu-id="8c723-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="8c723-112">Chọn **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="8c723-112">Select **Search**.</span></span> <span data-ttu-id="8c723-113">Các hoạt động sẽ xuất hiện bên dưới **kết quả**.</span><span class="sxs-lookup"><span data-stu-id="8c723-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="8c723-114">Chọn **lọc kết quả**, rồi nhập **Set-Mailbox** trong trường bộ lọc **hoạt động** .</span><span class="sxs-lookup"><span data-stu-id="8c723-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="8c723-115">Điều này trả về tất cả các hoạt động **đặt hộp thư** .</span><span class="sxs-lookup"><span data-stu-id="8c723-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="8c723-116">Để xem chi tiết, hãy chọn một hoạt động, rồi chọn **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="8c723-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="8c723-117">Bên dưới **tham số** , bạn có thể thấy địa chỉ email chuyển tiếp đã được đặt trên hộp thư.</span><span class="sxs-lookup"><span data-stu-id="8c723-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="8c723-118">**Userid** đại diện cho người dùng đã thiết lập việc chuyển tiếp bên ngoài trên hộp thư.</span><span class="sxs-lookup"><span data-stu-id="8c723-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="8c723-119">Để tìm hiểu thêm, hãy xem [Tìm kiếm Nhật ký kiểm tra Office 365 để khắc phục các kịch bản phổ biến](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="8c723-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>