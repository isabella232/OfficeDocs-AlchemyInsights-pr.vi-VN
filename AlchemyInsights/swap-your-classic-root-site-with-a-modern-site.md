---
title: Trao đổi trang web gốc cổ điển của bạn với một trang web hiện đại
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501101"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="7720c-102">Trao đổi trang web gốc cổ điển của bạn với một trang web hiện đại</span><span class="sxs-lookup"><span data-stu-id="7720c-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="7720c-103">Nếu môi trường của bạn đã được thiết lập trước khi tháng tư 2019, bạn có thể thay đổi trang web gốc của bạn vào một trang web hiện đại bằng cách sử dụng Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7720c-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="7720c-104">Nếu bạn có một trang web khác mà bạn muốn sử dụng như là trang web gốc của bạn, bạn có thể thay thế (trao đổi) gốc trang web với nó.</span><span class="sxs-lookup"><span data-stu-id="7720c-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="7720c-105">Sử dụng [Gọi SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để trao đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang web gốc.</span><span class="sxs-lookup"><span data-stu-id="7720c-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7720c-106">Sẵn sàng cho cả hai nhóm trang web (không kết nối với một nhóm) và trang web thông tin liên lạc.</span><span class="sxs-lookup"><span data-stu-id="7720c-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="7720c-107">Bổ sung khả năng sẽ được giới thiệu sớm mà sẽ cho phép bạn tiếp tục sử dụng nội dung trên trang web, nhưng chuyển đổi trang web hiện có để một trang web thông tin liên lạc.</span><span class="sxs-lookup"><span data-stu-id="7720c-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="7720c-108">Những khả năng sẽ được cuộn ra dần dần.</span><span class="sxs-lookup"><span data-stu-id="7720c-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="7720c-109">Tiếp tục để kiểm tra xem Trung tâm thông báo Office 365 bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="7720c-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7720c-110">Các vấn đề được biết đến với các trang web trao đổi</span><span class="sxs-lookup"><span data-stu-id="7720c-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="7720c-111">Trang web mục tiêu có thể trả lại một lỗi "không tìm thấy" (HTTP 404) cho một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="7720c-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7720c-112">Nội dung sẽ cần phải được recrawled để cập nhật danh mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="7720c-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7720c-113">Có không có bước hướng dẫn sử dụng yêu cầu - điều này sẽ được thực hiện tự động.</span><span class="sxs-lookup"><span data-stu-id="7720c-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="7720c-114">Bất cứ điều gì phụ thuộc vào các liên kết "tĩnh" (chẳng hạn như đồng bộ hóa tập tin và OneNote files) sẽ cần phải được sửa chữa bằng tay.</span><span class="sxs-lookup"><span data-stu-id="7720c-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7720c-115">Nếu trang web mã nguồn là một trang web tổ chức tin tức, Cập Nhật URL.</span><span class="sxs-lookup"><span data-stu-id="7720c-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="7720c-116">Nhận được một danh sách tất cả các trang web tin tức tổ chức.</span><span class="sxs-lookup"><span data-stu-id="7720c-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="7720c-117">Dự án máy chủ trang web có thể cần phải được xác nhận để đảm bảo rằng họ vẫn còn liên kết một cách chính xác.</span><span class="sxs-lookup"><span data-stu-id="7720c-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





