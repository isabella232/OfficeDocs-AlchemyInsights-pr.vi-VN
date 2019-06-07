---
title: Xác định địa chỉ IP và các khách hàng trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752081"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="99dcf-102">Xác định địa chỉ IP và các khách hàng trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="99dcf-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="99dcf-103">Địa chỉ IP tương ứng với một hoạt động của một người dùng hay quản trị được thể hiện trong Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="99dcf-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="99dcf-104">Thông tin khách hàng cũng đã đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="99dcf-104">The client information is also logged.</span></span> <span data-ttu-id="99dcf-105">Dưới đây là các bước để xác định các thông tin như vậy</span><span class="sxs-lookup"><span data-stu-id="99dcf-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="99dcf-106">Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="99dcf-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="99dcf-107">Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="99dcf-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="99dcf-108">Nếu bạn đang quan tâm đến một hoạt động cụ thể, chọn nó từ danh sách **các hoạt động** .</span><span class="sxs-lookup"><span data-stu-id="99dcf-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="99dcf-109">Nếu không, tất cả các hoạt động sẽ được trả lại cho người dùng lựa chọn (cài đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="99dcf-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="99dcf-110">**Lưu ý**: một số hoạt động có thể không có sẵn trong menu **hoạt động** ; Tuy nhiên, những người kiểm toán khoản mục này sẽ được trả lại nếu **Hiển thị kết quả cho tất cả các hoạt động** là lựa chọn (cài đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="99dcf-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="99dcf-111">Chỉ định tên người dùng trong lĩnh vực **người dùng** , chọn phạm vi ngày thích hợp cho các hoạt động, và sau đó nhấp vào **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="99dcf-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="99dcf-112">Trong kết quả, bạn có thể xem địa chỉ IP cho rằng hoạt động trong ngăn kết quả.</span><span class="sxs-lookup"><span data-stu-id="99dcf-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="99dcf-113">Chọn hồ sơ kiểm toán để xem thông tin chi tiết tại flyout **thông tin chi tiết** (ví dụ, khách hàng, người sử dụng thực hiện hành động, vv).</span><span class="sxs-lookup"><span data-stu-id="99dcf-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="99dcf-114">Để biết thêm chi tiết, hãy xem [Tìm địa chỉ IP của máy tính được sử dụng để truy cập vào một tài khoản bị xâm phạm](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="99dcf-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
