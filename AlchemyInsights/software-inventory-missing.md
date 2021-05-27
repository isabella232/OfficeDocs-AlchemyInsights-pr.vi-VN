---
title: Kiểm kê phần mềm bị thiếu hoặc không chính xác
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676589"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="857f6-102">Kiểm kê phần mềm bị thiếu hoặc không chính xác</span><span class="sxs-lookup"><span data-stu-id="857f6-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="857f6-103">Kiểm kê phần mềm trong Quản lý Mối đe dọa và Lỗ hổng (TVM) là một danh sách phần mềm đã biết trong tổ chức của bạn với Công thức Liệt kê Nền tảng Chung (CPE) chính thức.</span><span class="sxs-lookup"><span data-stu-id="857f6-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="857f6-104">Sản phẩm phần mềm không có CPE chính thức không có lỗ hổng được phát hành.</span><span class="sxs-lookup"><span data-stu-id="857f6-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="857f6-105">Hàng tồn kho cũng bao gồm các chi tiết như tên của nhà cung cấp, số lượng thiết bị tồn kho, mối đe dọa và số lượng thiết bị càng tiếp xúc.</span><span class="sxs-lookup"><span data-stu-id="857f6-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="857f6-106">Thay đổi phần mềm trên thiết bị thường được phản ánh trong cổng thông tin bảo mật trong vòng hai giờ.</span><span class="sxs-lookup"><span data-stu-id="857f6-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="857f6-107">Tuy nhiên, đôi khi có thể mất nhiều thời gian hơn.</span><span class="sxs-lookup"><span data-stu-id="857f6-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="857f6-108">Hiện không có cách nào để bắt buộc đồng bộ; đây là một đánh giá liên tục liên tục.</span><span class="sxs-lookup"><span data-stu-id="857f6-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="857f6-109">Nếu bạn thay đổi phần mềm và thay đổi không được phản ánh chính xác trong TVM sau 5 giờ, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="857f6-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="857f6-110">Kiểm tra phần bằng chứng phần mềm để tìm hiểu cách phần mềm được phát hiện.</span><span class="sxs-lookup"><span data-stu-id="857f6-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="857f6-111">Đảm bảo rằng phần mềm được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="857f6-111">Make sure that the software is supported.</span></span> <span data-ttu-id="857f6-112">Phần mềm có thể chỉ hiển thị ở cấp độ thiết bị ngay cả khi phần mềm hiện không được hỗ trợ Quản lý Mối đe dọa và Lỗ hổng.</span><span class="sxs-lookup"><span data-stu-id="857f6-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="857f6-113">Tuy nhiên, chỉ có dữ liệu có giới hạn là khả dụng.</span><span class="sxs-lookup"><span data-stu-id="857f6-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="857f6-114">Để biết các bước báo cáo không chính xác từ cổng thông tin, hãy [xem Báo cáo không chính xác.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="857f6-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="857f6-115">**Lưu** ý : Báo cáo không chính xác từ cổng thông tin MDE là kênh một chiều cho đến kỹ thuật.</span><span class="sxs-lookup"><span data-stu-id="857f6-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="857f6-116">Nếu sự cố này khẩn cấp, hãy mở thẻ hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="857f6-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="857f6-117">Để biết thêm thông tin, hãy [xem Kiểm kê phần mềm - Quản lý Mối đe dọa và Lỗ hổng.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="857f6-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>