---
title: Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716446"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="7b417-102">Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="7b417-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="7b417-103">Bạn có thể sử dụng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật của Microsoft 365 để xem các sự kiện quy tắc hộp thư đến (tạo, sửa đổi và xoá quy tắc hộp thư đến).</span><span class="sxs-lookup"><span data-stu-id="7b417-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="7b417-104">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7b417-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7b417-105">Đi tới trang**Tìm kiếm Nhật ký kiểm tra** **Tìm kiếm** > .</span><span class="sxs-lookup"><span data-stu-id="7b417-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="7b417-106">Chọn phạm vi ngày trong ngày **bắt đầu** và **ngày kết thúc** trường.</span><span class="sxs-lookup"><span data-stu-id="7b417-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="7b417-107">Trong **hoạt động hộp thư Exchange**, kiểm tra trường **hoạt động** được đặt **mới-inboxrule tạo/sửa đổi/kích hoạt/vô hiệu hoá quy tắc hộp thư**đến.</span><span class="sxs-lookup"><span data-stu-id="7b417-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="7b417-108">Nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="7b417-108">Click **Search**.</span></span>

<span data-ttu-id="7b417-109">Trong kết quả, chọn bản ghi kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="7b417-109">In the results, select an audit record.</span></span> <span data-ttu-id="7b417-110">Trong thông tin chi tiết flyout, hãy nhấp vào **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="7b417-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="7b417-111">Thông tin về các thiết đặt quy tắc hộp thư đến được hiển thị trong trường **tham số** .</span><span class="sxs-lookup"><span data-stu-id="7b417-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="7b417-112">Để biết thêm thông tin, xem [xác định nếu người dùng tạo quy tắc hộp thư đến](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="7b417-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
