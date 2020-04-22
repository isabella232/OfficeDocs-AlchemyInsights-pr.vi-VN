---
title: Xác định địa chỉ IP và khách hàng trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716410"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="aa671-102">Xác định địa chỉ IP và khách hàng trong Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="aa671-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="aa671-103">Địa chỉ IP tương ứng với một hoạt động của người dùng Microsoft 365 hoặc quản trị viên được hiển thị trong Nhật ký kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="aa671-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="aa671-104">Thông tin khách hàng cũng được ghi lại.</span><span class="sxs-lookup"><span data-stu-id="aa671-104">The client information is also logged.</span></span> <span data-ttu-id="aa671-105">Dưới đây là các bước để xác định thông tin đó</span><span class="sxs-lookup"><span data-stu-id="aa671-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="aa671-106">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="aa671-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="aa671-107">Đi tới trang**Tìm kiếm Nhật ký kiểm tra** **Tìm kiếm** > .</span><span class="sxs-lookup"><span data-stu-id="aa671-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="aa671-108">Nếu bạn quan tâm đến một hoạt động cụ thể, hãy chọn nó từ danh sách **hoạt động** .</span><span class="sxs-lookup"><span data-stu-id="aa671-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="aa671-109">Nếu không, tất cả các hoạt động sẽ được trả lại cho người dùng đã chọn (cài đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="aa671-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="aa671-110">**Lưu ý**: một số hoạt động có thể không có sẵn trong menu **hoạt động** ; Tuy nhiên, các mục kiểm tra sẽ được trả lại nếu **Hiển thị kết quả cho tất cả các hoạt động** được chọn (cài đặt mặc định).</span><span class="sxs-lookup"><span data-stu-id="aa671-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="aa671-111">Chỉ định tên người dùng trong trường **người sử dụng** , chọn phạm vi ngày thích hợp cho hoạt động, và sau đó bấm **Tìm kiếm**.</span><span class="sxs-lookup"><span data-stu-id="aa671-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="aa671-112">Trong kết quả, bạn có thể thấy địa chỉ IP cho hoạt động đó trong ngăn kết quả.</span><span class="sxs-lookup"><span data-stu-id="aa671-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="aa671-113">Chọn bản ghi kiểm tra để xem thông tin chi tiết trong mục thả xuống **thông** tin (ví dụ: khách hàng, người dùng đã thực hiện hành động, v.v.).</span><span class="sxs-lookup"><span data-stu-id="aa671-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="aa671-114">Để biết thêm thông tin, hãy xem [Tìm địa chỉ IP của máy tính được sử dụng để truy cập tài khoản bị xâm phạm](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="aa671-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
