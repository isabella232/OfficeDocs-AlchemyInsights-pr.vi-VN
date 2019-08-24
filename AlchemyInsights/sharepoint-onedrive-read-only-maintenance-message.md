---
title: Chỉ đọc cho các thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620745"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="16231-102">Chỉ đọc cho các thông báo bảo trì khi cố gắng sử dụng SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="16231-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="16231-103">Người dùng có thể nhận được một tin nhắn **Chỉ đọc bảo trì** khi cố gắng sử dụng SharePoint hoặc OneDrive cho một trong các trường hợp sau.</span><span class="sxs-lookup"><span data-stu-id="16231-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="16231-104">Một kế hoạch hoặc hoạt động duy trì hoạt động.</span><span class="sxs-lookup"><span data-stu-id="16231-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="16231-105">Kiểm tra cho họ bằng cách điều hướng đến [Trung tâm tin nhắn](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="16231-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="16231-106">Một ưu tiên cao, hoạt động sự cố có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="16231-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="16231-107">Kiểm tra bất kỳ tư vấn/sự cố bằng cách điều hướng đến [Dịch vụ sức khỏe](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="16231-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="16231-108">Một tiểu tự chữa bệnh phục hồi tình huống có thể xảy ra do sự kiện bất ngờ nào trên các máy chủ đó có thể cuối cùng trong chưa đầy 30 phút hoặc lâu hơn.</span><span class="sxs-lookup"><span data-stu-id="16231-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="16231-109">Không có không có trung tâm tin nhắn hoặc dịch vụ sức khỏe bài viết cho những phục hồi nhỏ, nhưng bạn nên trở lại bình thường rất sớm.</span><span class="sxs-lookup"><span data-stu-id="16231-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="16231-110">Trong những dịp rất ít chúng tôi quan sát thấy rằng một trong ba trường hợp nêu trên có là nguyên nhân, và dịch vụ đã được khôi phục, nhưng bộ nhớ cache trình duyệt của người dùng đã bị xoá sổ.</span><span class="sxs-lookup"><span data-stu-id="16231-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="16231-111">Hãy cố gắng để xóa bộ nhớ cache của trình duyệt trước khi điều hướng đến trang web.</span><span class="sxs-lookup"><span data-stu-id="16231-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="16231-112">Trong trình duyệt Microsoft Edge, chọn **Settings**và sau đó chọn **quyền riêng tư và bảo mật**.</span><span class="sxs-lookup"><span data-stu-id="16231-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="16231-113">**Rõ ràng đang duyệt**, chọn **lựa chọn những gì để xóa**.</span><span class="sxs-lookup"><span data-stu-id="16231-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="16231-114">Chọn **cookie và dữ liệu trang web đã lưu**, và chọn **xóa**.</span><span class="sxs-lookup"><span data-stu-id="16231-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="16231-115">Các bước này có thể khác biệt khi sử dụng các trình duyệt khác như Mozilla Firefox hoặc Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="16231-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="16231-116">Một tùy chọn khác sẽ là mở OneDrive hoặc SharePoint trang web của bạn trong một cửa sổ InPrivate mới.</span><span class="sxs-lookup"><span data-stu-id="16231-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>