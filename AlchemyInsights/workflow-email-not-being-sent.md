---
title: Luồng công việc email không được gửi
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766155"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="ddaa9-102">Luồng công việc email không được gửi cho một danh sách SharePoint hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="ddaa9-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="ddaa9-103">Email từ luồng công việc không được gửi đến tất cả người dùng hoặc chỉ người dùng cụ thể hoặc bạn thấy lỗi **thư email không được gửi. Đảm bảo rằng e-mail có người nhận hợp lệ**.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="ddaa9-104">Kiểm tra xem người dùng tồn tại trong **tất cả mọi người** quyền nhóm (danh sách thông tin người dùng) cho bộ sưu tập trang web đó.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ddaa9-105">Mẫu URL trực tiếp:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/nhân .aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ddaa9-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="ddaa9-106">Nếu người dùng không tồn tại, đảm bảo rằng người dùng được đăng nhập vào trang.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="ddaa9-107">Nếu đó là người dùng bên ngoài, hãy đảm bảo rằng lời mời của họ đã được chấp nhận.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="ddaa9-108">Nếu người dùng tồn tại trong nhóm quyền, đảm bảo rằng địa chỉ email là chính xác.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="ddaa9-109">Nếu địa chỉ email của người dùng không được đặt ở đây, sau đó tạo một cảnh báo mẫu cho người dùng đó buộc đồng bộ hoá tài khoản người dùng từ hồ sơ người dùng của SharePoint vào bộ sưu tập trang web này.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ddaa9-110">Email từ luồng công việc được gửi đến quản trị viên bộ sưu tập trang web nhưng không cho người dùng khác và xem lỗi **http bị cấm <span>https:</span>//URL/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="ddaa9-111">Xem [truy cập bị từ chối khi bạn gửi một email đến một nhóm SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="ddaa9-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="ddaa9-112">Ngoài ra, xác minh rằng tính năng bộ sưu tập trang web **chế độ khoá truy cập giới hạn cho phép người dùng** không hoạt động.</span><span class="sxs-lookup"><span data-stu-id="ddaa9-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="ddaa9-113">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="ddaa9-113">Related topics</span></span>
<span data-ttu-id="ddaa9-114">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ddaa9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ddaa9-115">Tạo Flow</span><span class="sxs-lookup"><span data-stu-id="ddaa9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ddaa9-116">SharePoint và Flow</span><span class="sxs-lookup"><span data-stu-id="ddaa9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


