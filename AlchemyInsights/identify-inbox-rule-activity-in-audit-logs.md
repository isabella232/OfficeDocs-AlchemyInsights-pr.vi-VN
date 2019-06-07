---
title: Xác định các hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755059"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="b0d08-102">Xác định các hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="b0d08-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="b0d08-103">Bạn có thể sử dụng kiểm toán đăng nhập tìm kiếm trong an ninh & tuân thủ trung tâm để xem sự kiện quy tắc hộp thư đến (tạo, chỉnh sửa và xoá quy tắc hộp thư đến).</span><span class="sxs-lookup"><span data-stu-id="b0d08-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="b0d08-104">Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b0d08-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b0d08-105">Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="b0d08-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b0d08-106">Chọn phạm vi ngày trong các **ngày bắt đầu** và **ngày kết thúc** .</span><span class="sxs-lookup"><span data-stu-id="b0d08-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="b0d08-107">Theo **Hoạt động giao lưu hộp thư**, xác minh các lĩnh vực **hoạt động** được thiết lập để **quy tắc hộp thư đến mới-InboxRule tạo/sửa đổi/cho phép/vô hiệu hóa**.</span><span class="sxs-lookup"><span data-stu-id="b0d08-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="b0d08-108">Nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="b0d08-108">Click **Search**.</span></span>

<span data-ttu-id="b0d08-109">Trong các kết quả, hãy chọn một hồ sơ kiểm toán.</span><span class="sxs-lookup"><span data-stu-id="b0d08-109">In the results, select an audit record.</span></span> <span data-ttu-id="b0d08-110">Trong flyout chi tiết, bấm vào **Thêm thông tin**.</span><span class="sxs-lookup"><span data-stu-id="b0d08-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b0d08-111">Thông tin về các thiết đặt quy tắc hộp thư đến sẽ được hiển thị trong lĩnh vực **thông số** .</span><span class="sxs-lookup"><span data-stu-id="b0d08-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="b0d08-112">Để biết thêm chi tiết, xem [Determining nếu người dùng tạo quy tắc hộp thư đến](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="b0d08-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
