---
title: Email dòng công việc không được gửi đi
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749031"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="096ef-102">Email dòng công việc không được gửi cho một danh sách hoặc thư viện SharePoint</span><span class="sxs-lookup"><span data-stu-id="096ef-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="096ef-103">Email từ dòng công việc không được gửi đến tất cả người dùng hoặc chỉ những người dùng cụ thể hoặc bạn thấy **thông báo lỗi email không thể gửi được. Hãy đảm bảo email có một người nhận hợp lệ**.</span><span class="sxs-lookup"><span data-stu-id="096ef-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="096ef-104">Kiểm tra xem người dùng có tồn tại trong nhóm quyền **tất cả mọi người** (danh sách thông tin người dùng) cho tuyển tập trang đó hay không.</span><span class="sxs-lookup"><span data-stu-id="096ef-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="096ef-105">URL trực tiếp mẫu: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/người. aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="096ef-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="096ef-106">Nếu người dùng không tồn tại, hãy đảm bảo rằng người dùng đã đăng nhập vào trang.</span><span class="sxs-lookup"><span data-stu-id="096ef-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="096ef-107">Nếu đó là một người dùng bên ngoài, hãy đảm bảo rằng lời mời của họ đã được chấp nhận.</span><span class="sxs-lookup"><span data-stu-id="096ef-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="096ef-108">Nếu người dùng không tồn tại trong nhóm quyền, hãy đảm bảo rằng địa chỉ email chính xác.</span><span class="sxs-lookup"><span data-stu-id="096ef-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="096ef-109">Nếu địa chỉ email của người dùng không được đặt ở đây, sau đó tạo một cảnh báo mẫu cho người dùng đó lực lượng đồng bộ của tài khoản người dùng đó từ hồ sơ người dùng của SharePoint vào tuyển tập trang này.</span><span class="sxs-lookup"><span data-stu-id="096ef-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="096ef-110">Email từ dòng công việc được gửi đến người quản trị tuyển tập trang nhưng không cho người dùng khác và xem lỗi **http đã cấm cho <span>https:</span>//url/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="096ef-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="096ef-111">Xem [Access bị từ chối khi bạn gửi email đến một nhóm SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="096ef-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="096ef-112">Ngoài ra, hãy xác minh rằng tính năng của bộ sưu tập trang **chế độ có quyền hạn chế của người dùng truy nhập** không hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="096ef-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="096ef-113">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="096ef-113">Related topics</span></span>
<span data-ttu-id="096ef-114">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="096ef-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="096ef-115">Tạo dòng</span><span class="sxs-lookup"><span data-stu-id="096ef-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="096ef-116">SharePoint và dòng</span><span class="sxs-lookup"><span data-stu-id="096ef-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


