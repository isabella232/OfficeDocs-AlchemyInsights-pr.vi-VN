---
title: Xác định địa chỉ IP và máy khách trong Nhật ký kiểm tra
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668332"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="543cd-102">Xác định địa chỉ IP và máy khách trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="543cd-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="543cd-103">Địa chỉ IP tương ứng với một hoạt động bởi một người dùng Microsoft 365 hoặc người quản trị được hiển thị trong Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="543cd-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="543cd-104">Thông tin máy khách cũng được ghi nhật ký.</span><span class="sxs-lookup"><span data-stu-id="543cd-104">The client information is also logged.</span></span> <span data-ttu-id="543cd-105">Sau đây là các bước để xác định thông tin đó</span><span class="sxs-lookup"><span data-stu-id="543cd-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="543cd-106">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="543cd-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="543cd-107">Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="543cd-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="543cd-108">Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn nó từ danh sách **hoạt động** .</span><span class="sxs-lookup"><span data-stu-id="543cd-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="543cd-109">Nếu không, tất cả các hoạt động sẽ được trả về cho người dùng được chọn (thiết đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="543cd-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="543cd-110">**Lưu ý**: một số hoạt động có thể không sẵn dùng trong menu **hoạt động** ; Tuy nhiên, những mục kiểm tra này sẽ được trả về nếu **Hiển thị kết quả cho tất cả các hoạt động** được chọn (thiết đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="543cd-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="543cd-111">Xác định tên người dùng trong trường **người dùng** , chọn phạm vi ngày thích hợp cho hoạt động rồi sau đó bấm **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="543cd-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="543cd-112">Trong kết quả, bạn có thể thấy địa chỉ IP cho hoạt động đó trong ngăn kết quả.</span><span class="sxs-lookup"><span data-stu-id="543cd-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="543cd-113">Chọn bản ghi kiểm tra để xem thông tin chi tiết trong các **chi tiết** đã phát ra (ví dụ, máy khách, người dùng thực hiện hành động, v.v.).</span><span class="sxs-lookup"><span data-stu-id="543cd-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="543cd-114">Để biết thêm thông tin, hãy xem [Tìm địa chỉ IP của máy tính được dùng để truy nhập vào tài khoản bị xâm](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)phạm.</span><span class="sxs-lookup"><span data-stu-id="543cd-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
