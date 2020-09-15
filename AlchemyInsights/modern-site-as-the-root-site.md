---
title: Site hiện đại như site gốc
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666892"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6353e-102">Site hiện đại như site gốc</span><span class="sxs-lookup"><span data-stu-id="6353e-102">Modern site as root site</span></span>

<span data-ttu-id="6353e-103">Chúng tôi đã bắt đầu triển khai một tính năng mới sẽ cho phép bạn [hoán đổi site gốc site cổ điển của bạn với site hiện đại](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="6353e-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="6353e-104">Sử dụng cuộc [gọi-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang gốc.</span><span class="sxs-lookup"><span data-stu-id="6353e-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6353e-105">Sẵn dùng cho cả site nhóm (không được kết nối với một nhóm) và site liên lạc.</span><span class="sxs-lookup"><span data-stu-id="6353e-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="6353e-106">Không xóa site gốc cổ điển của bạn để tạo một site liên lạc hiện đại.</span><span class="sxs-lookup"><span data-stu-id="6353e-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6353e-107">Điều này không được Microsoft hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="6353e-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6353e-108">Việc xóa site gốc sẽ làm cho tất cả các site SharePoint trong tổ chức của bạn không thể truy nhập được tất cả người dùng, cho đến khi bạn khôi phục site hoặc tạo một site mới tại cùng một URL.</span><span class="sxs-lookup"><span data-stu-id="6353e-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6353e-109">Chúng tôi sẽ giao tiếp tính năng này thông qua Trung tâm thông báo.</span><span class="sxs-lookup"><span data-stu-id="6353e-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6353e-110">Bạn nên trông đợi tính năng này sẽ được bật trong đối tượng thuê của bạn một thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="6353e-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6353e-111">Các vấn đề đã biết với việc trao đổi site</span><span class="sxs-lookup"><span data-stu-id="6353e-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6353e-112">Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="6353e-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6353e-113">Nội dung sẽ cần được recrawled để cập nhật chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="6353e-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6353e-114">Không có bước thủ công nào cần thiết ở đây, điều này sẽ được thực hiện tự động.</span><span class="sxs-lookup"><span data-stu-id="6353e-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6353e-115">Bất kỳ điều gì phụ thuộc vào các nối kết "tĩnh" (chẳng hạn như tệp đồng bộ tệp và tệp OneNote) sẽ cần được sửa chữa theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="6353e-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6353e-116">Các trang web dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết đúng.</span><span class="sxs-lookup"><span data-stu-id="6353e-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
