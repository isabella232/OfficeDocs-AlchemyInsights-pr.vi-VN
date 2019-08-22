---
title: Xác định sự kiện thông báo xóa trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539231"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="2be6e-102">Nhật ký kiểm tra cho các thư email đã xoá</span><span class="sxs-lookup"><span data-stu-id="2be6e-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="2be6e-103">Bắt đầu từ năm 2019, Microsoft là chuyển vào hộp thư kiểm tra đăng nhập theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="2be6e-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="2be6e-104">Nếu không, để xem xét xóa các sự kiện tin nhắn cho một người dùng cụ thể, bạn cần bật bằng tay các hành động delete đối với kiểm toán.</span><span class="sxs-lookup"><span data-stu-id="2be6e-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="2be6e-105">Nếu hộp kiểm toán đăng nhập đã được kích hoạt cho tổ chức của bạn hoặc cho người dùng cụ thể, hãy làm theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="2be6e-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="2be6e-106">Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2be6e-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2be6e-107">Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2be6e-108">Chọn phạm vi ngày trong các **ngày bắt đầu** và **ngày kết thúc** .</span><span class="sxs-lookup"><span data-stu-id="2be6e-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="2be6e-109">Chỉ định tên đăng nhập cho người dùng mà bạn muốn để điều tra (người dùng xóa các mục).</span><span class="sxs-lookup"><span data-stu-id="2be6e-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="2be6e-110">Trong lĩnh vực **hoạt động** , lựa chọn **đã bị xoá thư khỏi thư mục mục đã xoá** và **chuyển thư đến thư mục mục đã xoá**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="2be6e-111">Nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-111">Click **Search**.</span></span>

<span data-ttu-id="2be6e-112">Trong các kết quả, hãy chọn một hồ sơ kiểm toán.</span><span class="sxs-lookup"><span data-stu-id="2be6e-112">In the results, select an audit record.</span></span> <span data-ttu-id="2be6e-113">Trong flyout chi tiết, bấm vào **Thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2be6e-114">Các thông tin bổ sung về mục đã xoá (ví dụ, dòng tiêu đề và vị trí các mục khi đã bị xóa) sẽ được hiển thị trong lĩnh vực **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="2be6e-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="2be6e-115">Bất động sản **ClientInfoString** sẽ hiển thị nếu việc xoá bỏ xảy ra trong Outlook, Outlook trên web (trước đây gọi là Outlook Web App), hoặc bất kỳ thiết bị nào khác.</span><span class="sxs-lookup"><span data-stu-id="2be6e-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="2be6e-116">Để biết thêm chi tiết, hãy xem [Determining người thiết lập email chuyển tiếp cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="2be6e-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="2be6e-117">**Lưu ý**: bạn không thể truy xuất khoản mục đã xóa bằng cách sử dụng tính năng đăng nhập kiểm toán.</span><span class="sxs-lookup"><span data-stu-id="2be6e-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="2be6e-118">Để truy lục thư đã xoá trong Outlook trên web, hãy xem [khôi phục đã xoá các mục trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="2be6e-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
