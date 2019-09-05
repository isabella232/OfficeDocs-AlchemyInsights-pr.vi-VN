---
title: Trang web hiện đại như là trang web gốc
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753926"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="90cd2-102">Trang web hiện đại như trang web gốc</span><span class="sxs-lookup"><span data-stu-id="90cd2-102">Modern site as root site</span></span>

<span data-ttu-id="90cd2-103">Chúng tôi đã bắt đầu triển khai một tính năng mới mà sẽ cho phép bạn hoán đổi trang web gốc trang web [cổ điển của bạn với một trang web hiện đại](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="90cd2-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="90cd2-104">Sử dụng [gọi SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web trong khi lưu trữ các trang web ban đầu.</span><span class="sxs-lookup"><span data-stu-id="90cd2-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="90cd2-105">Có sẵn cho cả hai trang web nhóm (không được kết nối với một nhóm) và trang web truyền thông.</span><span class="sxs-lookup"><span data-stu-id="90cd2-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="90cd2-106">Không xóa trang web gốc cổ điển của bạn để tạo ra một trang web truyền thông hiện đại.</span><span class="sxs-lookup"><span data-stu-id="90cd2-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="90cd2-107">Điều này không được hỗ trợ bởi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="90cd2-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="90cd2-108">Xóa các trang web gốc sẽ làm cho tất cả các trang web SharePoint trong tổ chức của bạn không thể truy nhập cho tất cả người dùng, cho đến khi bạn khôi phục lại các trang web hoặc tạo ra một trang web mới tại cùng một URL.</span><span class="sxs-lookup"><span data-stu-id="90cd2-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="90cd2-109">Chúng tôi sẽ giao tiếp tính năng này thông qua Trung tâm tin nhắn.</span><span class="sxs-lookup"><span data-stu-id="90cd2-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="90cd2-110">Bạn nên mong đợi tính năng được bật trong thuê của bạn ngay.</span><span class="sxs-lookup"><span data-stu-id="90cd2-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="90cd2-111">Các vấn đề với trao đổi trang web</span><span class="sxs-lookup"><span data-stu-id="90cd2-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="90cd2-112">Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="90cd2-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="90cd2-113">Nội dung cần phải được thu thập lại để cập nhật chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="90cd2-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="90cd2-114">Không có hướng dẫn sử dụng bước cần thiết ở đây, điều này sẽ được thực hiện tự động.</span><span class="sxs-lookup"><span data-stu-id="90cd2-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="90cd2-115">Bất cứ điều gì phụ thuộc vào "tĩnh" liên kết (chẳng hạn như tập tin Sync và OneNote tập tin) sẽ cần phải được sửa chữa thủ công.</span><span class="sxs-lookup"><span data-stu-id="90cd2-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="90cd2-116">Trang web máy chủ dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết chính xác.</span><span class="sxs-lookup"><span data-stu-id="90cd2-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
