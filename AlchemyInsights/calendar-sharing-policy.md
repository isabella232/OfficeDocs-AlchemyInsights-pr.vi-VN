---
title: 618 chính sách chia sẻ lịch
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373021"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="396b5-102">Lỗi chính sách khi chia sẻ lịch</span><span class="sxs-lookup"><span data-stu-id="396b5-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="396b5-103">Thực hiện một trong những điều sau, nếu phù hợp với tình huống của bạn:</span><span class="sxs-lookup"><span data-stu-id="396b5-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="396b5-104">Kết nối với Exchange Online bằng cách sử dụng PowerShell từ xa.</span><span class="sxs-lookup"><span data-stu-id="396b5-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="396b5-105">Để biết thêm thông tin, xem [kết nối với Exchange Online sử dụng PowerShell từ xa](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="396b5-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="396b5-106">Trên máy chủ tại chỗ, mở Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="396b5-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="396b5-107">Xác định chính sách chia sẻ được gán cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="396b5-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="396b5-108">Để thực hiện việc này, hãy chạy lệnh sau và lưu ý chính sách trả lại:</span><span class="sxs-lookup"><span data-stu-id="396b5-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="396b5-109">Cập Nhật chính sách chia sẻ cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="396b5-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="396b5-110">Caranya sebagai berikut:</span><span class="sxs-lookup"><span data-stu-id="396b5-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="396b5-111">Mở Trung tâm quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="396b5-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="396b5-112">Bấm **tổ chức**, và sau đó bấm đúp vào chính sách được gán cho người dùng trong **chia sẻ cá nhân**.</span><span class="sxs-lookup"><span data-stu-id="396b5-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="396b5-113">Đây là chính sách được trả về trong bước 2.</span><span class="sxs-lookup"><span data-stu-id="396b5-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="396b5-114">Trên trang quy tắc chia sẻ, chọn mức độ chia sẻ lịch mà bạn muốn cho phép theo **chỉ định thông tin bạn muốn chia sẻ**; bấm vào **lưu**.</span><span class="sxs-lookup"><span data-stu-id="396b5-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="396b5-115">Để biết thêm thông tin xem: ["chính sách không cho phép cấp quyền ở mức này cho một hoặc nhiều người nhận" lỗi khi người dùng cố gắng chia sẻ lịch](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="396b5-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
