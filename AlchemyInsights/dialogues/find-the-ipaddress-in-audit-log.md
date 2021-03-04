---
title: Tìm địa chỉ IP trong Nhật ký kiểm tra
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430256"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="52304-102">Tìm địa chỉ IP trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="52304-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="52304-103">Địa chỉ IP tương ứng với một hoạt động do một người dùng hoặc người quản trị thực hiện được hiển thị trong Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="52304-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="52304-104">Thông tin máy khách cũng được ghi nhật ký.</span><span class="sxs-lookup"><span data-stu-id="52304-104">The client information is also logged.</span></span> <span data-ttu-id="52304-105">Sau đây là cách xác định địa chỉ IP:</span><span class="sxs-lookup"><span data-stu-id="52304-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="52304-106">Đi đến [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="52304-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="52304-107">Chọn **Tìm**  >  **[kiếm Nhật ký kiểm](https://go.microsoft.com/fwlink/?linkid=2103759)** tra.</span><span class="sxs-lookup"><span data-stu-id="52304-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="52304-108">Nếu bạn thấy thông báo rằng bạn cần bật kiểm định, hãy tiếp tục và bật tính năng này ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="52304-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="52304-109">Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể kéo dữ liệu từ ngày trước đó.</span><span class="sxs-lookup"><span data-stu-id="52304-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="52304-110">Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn nó từ danh sách **hoạt động** ; Nếu không, theo mặc định, tất cả các hoạt động sẽ được trả về cho người dùng được chọn.</span><span class="sxs-lookup"><span data-stu-id="52304-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="52304-111">Lưu ý rằng một số hoạt động có thể không sẵn dùng để lựa chọn từ menu **hoạt động** ; Tuy nhiên, những mục kiểm tra này sẽ được trả về nếu **Hiển thị kết quả cho tất cả các hoạt động** được chọn (thiết đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="52304-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="52304-112">Xác định phạm vi ngày và trong trường **người dùng** , chọn tên người dùng cho người dùng mà bạn muốn điều tra.</span><span class="sxs-lookup"><span data-stu-id="52304-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="52304-113">Chọn **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="52304-113">Select **Search**.</span></span> <span data-ttu-id="52304-114">Các hoạt động sẽ xuất hiện bên dưới **kết quả**.</span><span class="sxs-lookup"><span data-stu-id="52304-114">The activities appear under **Results**.</span></span> <span data-ttu-id="52304-115">Bạn có thể thấy địa chỉ IP cho từng hoạt động.</span><span class="sxs-lookup"><span data-stu-id="52304-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="52304-116">Để xem chi tiết, hãy chọn một hoạt động, rồi chọn **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="52304-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="52304-117">Để tìm hiểu thêm, hãy xem tìm kiếm [Nhật ký kiểm tra Office 365 để khắc phục các kịch bản phổ biến](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="52304-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>