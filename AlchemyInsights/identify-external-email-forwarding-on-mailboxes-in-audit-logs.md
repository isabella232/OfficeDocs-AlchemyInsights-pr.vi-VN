---
title: Xác định chuyển tiếp email bên ngoài trên các hộp thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696319"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="e06a5-102">Xác định khi chuyển tiếp email bên ngoài được đặt cấu hình trên hộp thư</span><span class="sxs-lookup"><span data-stu-id="e06a5-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="e06a5-103">Khi người dùng Microsoft 365 đặt cấu hình chuyển tiếp email bên ngoài trên một hộp thư, hoạt động được kiểm toán như là một phần của lệnh ghép ngắn **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e06a5-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="e06a5-104">Bạn có thể thấy hoạt động bằng cách sử dụng tính năng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="e06a5-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="e06a5-105">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e06a5-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e06a5-106">Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="e06a5-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e06a5-107">Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** .</span><span class="sxs-lookup"><span data-stu-id="e06a5-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e06a5-108">Bạn không cần phải xác định tên người dùng.</span><span class="sxs-lookup"><span data-stu-id="e06a5-108">You don't need to specify a username.</span></span> <span data-ttu-id="e06a5-109">Xác minh trường **hoạt động** được thiết lập để **Hiển thị kết quả cho tất cả các hoạt động**.</span><span class="sxs-lookup"><span data-stu-id="e06a5-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="e06a5-110">Bấm **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="e06a5-110">Click **Search**.</span></span>

<span data-ttu-id="e06a5-111">Trong kết quả, bấm vào **lọc kết quả** và gõ **Set-Mailbox** trong hộp bộ lọc hoạt động.</span><span class="sxs-lookup"><span data-stu-id="e06a5-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="e06a5-112">Chọn một bản ghi kiểm tra trong kết quả.</span><span class="sxs-lookup"><span data-stu-id="e06a5-112">Select an audit record in the results.</span></span> <span data-ttu-id="e06a5-113">Trong phần **thông tin chi tiết** , hãy bấm **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="e06a5-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="e06a5-114">Bạn phải xem chi tiết của từng bản ghi kiểm tra để xác định xem hoạt động có liên quan đến chuyển tiếp email hay không.</span><span class="sxs-lookup"><span data-stu-id="e06a5-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="e06a5-115">**ObjectID**: giá trị biệt danh của hộp thư đã được sửa đổi.</span><span class="sxs-lookup"><span data-stu-id="e06a5-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="e06a5-116">**Tham số**: chuyển tiếp biểu thị _địa chỉ email_ đích.</span><span class="sxs-lookup"><span data-stu-id="e06a5-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="e06a5-117">**Userid**: người dùng đã cấu hình chuyển tiếp email trên hộp thư trong trường **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="e06a5-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="e06a5-118">Để biết thêm thông tin, hãy xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e06a5-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
