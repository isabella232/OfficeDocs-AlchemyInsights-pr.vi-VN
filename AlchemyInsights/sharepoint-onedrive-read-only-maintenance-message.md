---
title: Chỉ đọc cho thư bảo trì khi tìm cách dùng SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670854"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="3fe87-102">Chỉ đọc cho thư bảo trì khi tìm cách dùng SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="3fe87-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="3fe87-103">Người dùng có thể nhận được thông báo **chỉ đọc để bảo trì** khi tìm cách sử dụng SharePoint hoặc OneDrive cho một trong các kịch bản sau đây.</span><span class="sxs-lookup"><span data-stu-id="3fe87-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="3fe87-104">Hoạt động bảo trì có lên kế hoạch hoặc hoạt động.</span><span class="sxs-lookup"><span data-stu-id="3fe87-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="3fe87-105">Kiểm tra chúng bằng cách dẫn hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="3fe87-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="3fe87-106">Một sự cố dịch vụ có ưu tiên cao, hiện hoạt có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="3fe87-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="3fe87-107">Kiểm tra bất kỳ sự cố nào/sự cố bằng cách dẫn hướng đến trạng thái [dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3fe87-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="3fe87-108">Một kịch bản phục hồi tự động nhỏ có thể xảy ra do bất kỳ sự kiện bất ngờ nào trên các máy chủ có thể kéo dưới 30 phút trở lên.</span><span class="sxs-lookup"><span data-stu-id="3fe87-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="3fe87-109">Không có trung tâm thông báo hoặc bài đăng trạng thái dịch vụ cho những recoback nhỏ nhưng bạn nên trở lại bình thường rất sớm.</span><span class="sxs-lookup"><span data-stu-id="3fe87-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="3fe87-110">Trong những dịp mà chúng tôi quan sát thấy rằng một trong ba tình huống được liệt kê ở trên là nguyên nhân và dịch vụ đã được khôi phục, nhưng bộ đệm ẩn trình duyệt người dùng chưa được dọn dẹp.</span><span class="sxs-lookup"><span data-stu-id="3fe87-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="3fe87-111">Vui lòng tìm cách xóa bộ đệm ẩn của trình duyệt trước khi dẫn hướng đến trang.</span><span class="sxs-lookup"><span data-stu-id="3fe87-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="3fe87-112">Trong trình duyệt Microsoft Edge của bạn, chọn **thiết đặt**, rồi chọn **quyền riêng tư và bảo mật**.</span><span class="sxs-lookup"><span data-stu-id="3fe87-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="3fe87-113">Trong phần **xóa bỏ duyệt**, chọn **chọn những điều cần xóa**.</span><span class="sxs-lookup"><span data-stu-id="3fe87-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="3fe87-114">Chọn **cookie và dữ liệu website đã lưu**, rồi chọn **xóa**.</span><span class="sxs-lookup"><span data-stu-id="3fe87-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="3fe87-115">Các bước này có thể khác nhau khi sử dụng các trình duyệt khác chẳng hạn như Mozilla Firefox hoặc Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="3fe87-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="3fe87-116">Một tùy chọn khác sẽ là mở site SharePoint hoặc OneDrive của bạn trong cửa sổ InPrivate mới.</span><span class="sxs-lookup"><span data-stu-id="3fe87-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>