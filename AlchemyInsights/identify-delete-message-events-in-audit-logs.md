---
title: Xác định xóa sự kiện thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716518"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="3719c-102">Nhật ký kiểm tra cho thư email đã xóa</span><span class="sxs-lookup"><span data-stu-id="3719c-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="3719c-103">Bắt đầu từ tháng 2019, Microsoft đang bật kiểm tra hộp thư đăng nhập theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="3719c-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="3719c-104">Nếu không, để xem lại xóa sự kiện tin nhắn cho một người dùng cụ thể, bạn cần phải bật thủ công các hành động xóa để kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="3719c-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="3719c-105">Nếu hộp kiểm tra ghi nhật ký đã được kích hoạt cho tổ chức của bạn hoặc cho người dùng cụ thể, hãy làm theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="3719c-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="3719c-106">Đăng nhập vào [Microsoft 365 bảo mật & tuân thủ trung tâm](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="3719c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="3719c-107">Nhấp vào **Tìm kiếm và điều tra** và chọn **Tìm kiếm Nhật ký kiểm tra**.</span><span class="sxs-lookup"><span data-stu-id="3719c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="3719c-108">Chọn phạm vi ngày trong ngày **bắt đầu** và **ngày kết thúc** trường.</span><span class="sxs-lookup"><span data-stu-id="3719c-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="3719c-109">Chỉ định tên người dùng mà bạn muốn điều tra (người dùng đã xoá các mục).</span><span class="sxs-lookup"><span data-stu-id="3719c-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="3719c-110">Trong trường **hoạt động** , chọn thư **đã xoá từ thư mục mục đã xoá** và **di chuyển thư vào thư mục mục đã xóa**.</span><span class="sxs-lookup"><span data-stu-id="3719c-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="3719c-111">Nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="3719c-111">Click **Search**.</span></span>

<span data-ttu-id="3719c-112">Trong kết quả, chọn bản ghi kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="3719c-112">In the results, select an audit record.</span></span> <span data-ttu-id="3719c-113">Trong thông tin chi tiết flyout, hãy nhấp vào **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="3719c-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="3719c-114">Thông tin bổ sung về mục đã xoá (ví dụ: dòng chủ đề và vị trí của mục khi nó đã bị xoá) được hiển thị trong trường **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="3719c-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="3719c-115">Thuộc tính **Clientinfostring** sẽ hiển thị nếu xóa xảy ra trong Outlook, Outlook trên web (trước đây được gọi là Outlook Web App) hoặc bất kỳ thiết bị nào khác.</span><span class="sxs-lookup"><span data-stu-id="3719c-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="3719c-116">Để biết thêm thông tin, xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="3719c-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="3719c-117">**Lưu ý**: bạn không thể truy xuất các mục đã xóa bằng tính năng Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="3719c-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="3719c-118">Để lấy các thư đã xóa trong Outlook trên web, hãy xem [khôi phục các mục đã xóa trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="3719c-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
