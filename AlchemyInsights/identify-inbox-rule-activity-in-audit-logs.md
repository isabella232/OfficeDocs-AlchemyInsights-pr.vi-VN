---
title: Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779073"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="d2da9-102">Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="d2da9-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="d2da9-103">Bạn có thể sử dụng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật của Microsoft 365 để xem các sự kiện về quy tắc hộp thư đến (tạo, sửa đổi và xóa bỏ quy tắc hộp thư đến).</span><span class="sxs-lookup"><span data-stu-id="d2da9-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="d2da9-104">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d2da9-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d2da9-105">Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="d2da9-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="d2da9-106">Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** .</span><span class="sxs-lookup"><span data-stu-id="d2da9-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="d2da9-107">Bên dưới **hoạt động của hộp thư Exchange**, hãy xác minh trường **hoạt động** được đặt là **mới-inboxrule tạo/chỉnh sửa/bật/tắt quy tắc hộp thư đến**.</span><span class="sxs-lookup"><span data-stu-id="d2da9-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="d2da9-108">Bấm **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="d2da9-108">Click **Search**.</span></span>

<span data-ttu-id="d2da9-109">Trong kết quả, hãy chọn một bản ghi kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="d2da9-109">In the results, select an audit record.</span></span> <span data-ttu-id="d2da9-110">Trong phần thông tin chi tiết, hãy bấm **xem thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="d2da9-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d2da9-111">Thông tin về thiết đặt quy tắc hộp thư đến được hiển thị trong trường **tham số** .</span><span class="sxs-lookup"><span data-stu-id="d2da9-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="d2da9-112">Để biết thêm thông tin, hãy xem [xác định nếu người dùng đã tạo một quy tắc hộp thư đến](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="d2da9-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
