---
title: Xác định xóa các sự kiện thư trong Nhật ký kiểm tra
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696571"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="a5fad-102">Nhật ký kiểm tra cho thư email đã xóa</span><span class="sxs-lookup"><span data-stu-id="a5fad-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="a5fad-103">Bắt đầu từ tháng một 2019, Microsoft đang bật tính năng ghi nhật ký kiểm tra hộp thư theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="a5fad-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="a5fad-104">Nếu không, để xem lại sự kiện xóa tin nhắn cho một người dùng cụ thể, bạn cần cho phép các hành động xóa để kiểm tra theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="a5fad-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="a5fad-105">Nếu Nhật ký kiểm tra hộp thư đã được kích hoạt cho tổ chức của bạn hoặc đối với người dùng cụ thể, hãy thực hiện theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="a5fad-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="a5fad-106">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="a5fad-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="a5fad-107">Bấm **Tìm kiếm và điều tra** và chọn **Tìm kiếm Nhật ký kiểm**tra.</span><span class="sxs-lookup"><span data-stu-id="a5fad-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="a5fad-108">Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** .</span><span class="sxs-lookup"><span data-stu-id="a5fad-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a5fad-109">Xác định tên người dùng cho người dùng mà bạn muốn điều tra (người dùng đã xóa các mục).</span><span class="sxs-lookup"><span data-stu-id="a5fad-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="a5fad-110">Trong trường **hoạt động** , chọn **thư đã xóa khỏi thư mục các mục đã xóa** và thư đã **chuyển vào thư mục các mục đã xóa**.</span><span class="sxs-lookup"><span data-stu-id="a5fad-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="a5fad-111">Bấm **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="a5fad-111">Click **Search**.</span></span>

<span data-ttu-id="a5fad-112">Trong kết quả, hãy chọn một bản ghi kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="a5fad-112">In the results, select an audit record.</span></span> <span data-ttu-id="a5fad-113">Trong phần thông tin chi tiết, hãy bấm **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="a5fad-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="a5fad-114">Thông tin bổ sung về mục đã xóa (ví dụ, dòng chủ đề và vị trí của mục khi thư đã bị xóa) được hiển thị trong trường **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="a5fad-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="a5fad-115">Thuộc tính **Clientinfostring** sẽ hiển thị nếu việc xóa đã xảy ra trong Outlook, Outlook trên web (trước đây gọi là Outlook Web App) hoặc bất kỳ thiết bị nào khác.</span><span class="sxs-lookup"><span data-stu-id="a5fad-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="a5fad-116">Để biết thêm thông tin, hãy xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="a5fad-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="a5fad-117">**Lưu ý**: bạn không thể truy xuất các mục đã xóa bằng tính năng Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="a5fad-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="a5fad-118">Để truy xuất thư đã xóa trong Outlook trên web, hãy xem [khôi phục các mục đã xóa trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="a5fad-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
