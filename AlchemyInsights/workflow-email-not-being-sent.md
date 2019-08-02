---
title: Quy trình làm việc email chưa được gửi
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059625"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="5165e-102">Quy trình làm việc email chưa được gửi</span><span class="sxs-lookup"><span data-stu-id="5165e-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="5165e-103">Email từ quy trình công việc sẽ không được gửi đến tất cả người dùng hoặc chỉ có người dùng cụ thể, hoặc bạn nhìn thấy các lỗi **thư e-mail không thể gửi. Đảm bảo rằng e-mail đã nhận hợp lệ**.</span><span class="sxs-lookup"><span data-stu-id="5165e-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="5165e-104">Kiểm tra nếu người dùng tồn tại trong **Tất cả mọi người** quyền nhóm (danh sách thông tin người dùng) cho rằng bộ sưu tập trang web.</span><span class="sxs-lookup"><span data-stu-id="5165e-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="5165e-105">Mẫu trực tiếp URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="5165e-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="5165e-106">Nếu người dùng không tồn tại, đảm bảo rằng người dùng được đăng nhập vào trang.</span><span class="sxs-lookup"><span data-stu-id="5165e-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="5165e-107">Nếu nó là một người dùng bên ngoài, đảm bảo rằng lời mời của họ đã được chấp nhận.</span><span class="sxs-lookup"><span data-stu-id="5165e-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="5165e-108">Nếu người dùng không tồn tại trong nhóm quyền, đảm bảo rằng địa chỉ email là chính xác.</span><span class="sxs-lookup"><span data-stu-id="5165e-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="5165e-109">Nếu địa chỉ email mà người dùng không được thiết lập ở đây, sau đó tạo ra một cảnh báo mẫu cho người dùng đó mà các lực lượng đồng bộ của tài khoản người dùng đó từ hồ sơ người dùng SharePoint bộ sưu tập trang web này.</span><span class="sxs-lookup"><span data-stu-id="5165e-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="5165e-110">Email từ quy trình công việc sẽ được gửi đến người quản trị bộ sưu tập trang web, nhưng không cho người dùng khác và xem lỗi \*\*HTTP Cấm để <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="5165e-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="5165e-111">Xem [Truy cập từ chối khi email được gửi đến nhóm](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="5165e-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="5165e-112">Ngoài ra, xác minh rằng không phải là tính năng bộ sưu tập trang web của **chế độ khoá cứng hạn chế truy cập người dùng cho phép** hoạt động.</span><span class="sxs-lookup"><span data-stu-id="5165e-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="5165e-113">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="5165e-113">Related topics</span></span>
- [<span data-ttu-id="5165e-114">Tạo ra dòng chảy</span><span class="sxs-lookup"><span data-stu-id="5165e-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5165e-115">SharePoint và dòng chảy</span><span class="sxs-lookup"><span data-stu-id="5165e-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


