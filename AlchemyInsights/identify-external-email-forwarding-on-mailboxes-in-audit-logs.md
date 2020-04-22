---
title: Xác định chuyển tiếp email bên ngoài trên hộp thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716482"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="1edca-102">Xác định khi chuyển tiếp email bên ngoài được cấu hình trên hộp thư</span><span class="sxs-lookup"><span data-stu-id="1edca-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="1edca-103">Khi người dùng Microsoft 365 cấu hình chuyển tiếp email bên ngoài vào hộp thư, hoạt động được kiểm toán là một phần của lệnh ghép ngắn **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="1edca-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="1edca-104">Bạn có thể xem hoạt động bằng cách sử dụng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="1edca-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="1edca-105">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1edca-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1edca-106">Đi tới trang**Tìm kiếm Nhật ký kiểm tra** **Tìm kiếm** > .</span><span class="sxs-lookup"><span data-stu-id="1edca-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="1edca-107">Chọn phạm vi ngày trong ngày **bắt đầu** và **ngày kết thúc** trường.</span><span class="sxs-lookup"><span data-stu-id="1edca-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1edca-108">Bạn không cần phải chỉ định tên người dùng.</span><span class="sxs-lookup"><span data-stu-id="1edca-108">You don't need to specify a username.</span></span> <span data-ttu-id="1edca-109">Kiểm tra trường **hoạt động** được đặt để **Hiển thị kết quả cho tất cả các hoạt động**.</span><span class="sxs-lookup"><span data-stu-id="1edca-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="1edca-110">Nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="1edca-110">Click **Search**.</span></span>

<span data-ttu-id="1edca-111">Trong kết quả, bấm **lọc kết quả** và loại **bộ hộp thư** trong hộp lọc hoạt động.</span><span class="sxs-lookup"><span data-stu-id="1edca-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="1edca-112">Chọn bản ghi kiểm tra trong kết quả.</span><span class="sxs-lookup"><span data-stu-id="1edca-112">Select an audit record in the results.</span></span> <span data-ttu-id="1edca-113">Trong hộp thả xuống **chi tiết** , hãy nhấp vào **thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="1edca-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="1edca-114">Bạn phải xem chi tiết của mỗi bản ghi kiểm tra để xác định nếu hoạt động liên quan đến chuyển tiếp email.</span><span class="sxs-lookup"><span data-stu-id="1edca-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="1edca-115">**ObjectID**: bí danh giá trị của hộp thư được thay đổi.</span><span class="sxs-lookup"><span data-stu-id="1edca-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="1edca-116">**Tham số**: giao nhận _dingsmtpaddress_ chỉ email địa chỉ đích.</span><span class="sxs-lookup"><span data-stu-id="1edca-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="1edca-117">**Userid**: người dùng đã định cấu hình chuyển tiếp email trên hộp thư trong trường **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="1edca-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="1edca-118">Để biết thêm thông tin, xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1edca-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
