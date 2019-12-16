---
title: Chỉ đọc cho thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051303"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="5ebaa-102">Chỉ đọc cho thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="5ebaa-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="5ebaa-103">Người dùng có thể nhận được thông báo **bảo trì chỉ đọc** khi cố gắng sử dụng SharePoint hoặc OneDrive cho một trong các trường hợp sau.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="5ebaa-104">Một hoạt động bảo trì kế hoạch hoặc hoạt động.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="5ebaa-105">Kiểm tra chúng bằng điều hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="5ebaa-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="5ebaa-106">Một sự cố dịch vụ ưu tiên cao, hoạt động có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="5ebaa-107">Kiểm tra bất kỳ lời khuyên/sự cố nào bằng việc điều hướng đến [dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5ebaa-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="5ebaa-108">Một tình huống khôi phục tự động chữa bệnh nhỏ có thể xảy ra do bất kỳ sự kiện bất ngờ trên các máy chủ có thể kéo ít hơn 30 phút hoặc lâu hơn.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="5ebaa-109">Không có trung tâm thông báo hoặc dịch vụ y tế bài viết cho các phục hồi nhỏ nhưng bạn nên trở lại bình thường rất sớm.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="5ebaa-110">Trong những dịp rất ít chúng tôi quan sát thấy rằng một trong ba kịch bản được liệt kê ở trên đã được nguyên nhân, và dịch vụ đã được khôi phục, nhưng bộ nhớ cache của trình duyệt người dùng đã không được xóa.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="5ebaa-111">Hãy cố gắng xóa bộ nhớ cache của trình duyệt trước khi điều hướng đến trang web.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="5ebaa-112">Trong trình duyệt Microsoft Edge, chọn **cài đặt**, sau đó chọn **quyền riêng tư và bảo mật**.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="5ebaa-113">Trong **xóa duyệt**, chọn **chọn nội dung cần xóa**.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="5ebaa-114">Chọn **cookie và dữ liệu trang web đã lưu**và chọn **xóa**.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="5ebaa-115">Các bước này có thể khác nhau khi sử dụng các trình duyệt khác như Mozilla Firefox hoặc Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="5ebaa-116">Một tùy chọn khác sẽ là mở trang web SharePoint của bạn hoặc OneDrive trong một cửa sổ InPrivate mới.</span><span class="sxs-lookup"><span data-stu-id="5ebaa-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>