---
title: Trao đổi site gốc cổ điển của bạn với site hiện đại
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691201"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="e907f-102">Trao đổi site gốc cổ điển của bạn với site hiện đại</span><span class="sxs-lookup"><span data-stu-id="e907f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="e907f-103">Nếu môi trường của bạn đã được thiết lập trước ngày 2019 tháng 4, bạn có thể thay đổi site gốc của bạn với một site hiện đại bằng cách sử dụng Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e907f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="e907f-104">Nếu bạn có một trang khác mà bạn muốn dùng làm site gốc của mình, bạn có thể thay thế [(hoán đổi) trang gốc](https://docs.microsoft.com/sharepoint/modern-root-site) với nó.</span><span class="sxs-lookup"><span data-stu-id="e907f-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="e907f-105">Sử dụng cuộc [gọi-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang gốc.</span><span class="sxs-lookup"><span data-stu-id="e907f-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e907f-106">Sẵn dùng cho cả site nhóm (không được kết nối với một nhóm) và site liên lạc.</span><span class="sxs-lookup"><span data-stu-id="e907f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="e907f-107">Các chức năng bổ sung sẽ sớm được giới thiệu sẽ cho phép bạn tiếp tục sử dụng nội dung trên trang, nhưng chuyển đổi site hiện có vào một site liên lạc.</span><span class="sxs-lookup"><span data-stu-id="e907f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="e907f-108">Những khả năng này sẽ được thực hiện dần dần.</span><span class="sxs-lookup"><span data-stu-id="e907f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="e907f-109">Tiếp tục kiểm tra Trung tâm thông báo cho các bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="e907f-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e907f-110">Các vấn đề đã biết với việc trao đổi site</span><span class="sxs-lookup"><span data-stu-id="e907f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="e907f-111">Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="e907f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e907f-112">Nội dung sẽ cần được recrawled để cập nhật chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="e907f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e907f-113">Không có bước thủ công nào cần thiết-điều này sẽ được tự động hoàn tất.</span><span class="sxs-lookup"><span data-stu-id="e907f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="e907f-114">Bất kỳ điều gì phụ thuộc vào các nối kết "tĩnh" (chẳng hạn như tệp đồng bộ tệp và tệp OneNote) sẽ cần được sửa chữa theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="e907f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e907f-115">Nếu trang nguồn là một trang tin tức tổ chức, hãy cập nhật URL.</span><span class="sxs-lookup"><span data-stu-id="e907f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="e907f-116">Lấy danh sách tất cả các trang tin tức của tổ chức.</span><span class="sxs-lookup"><span data-stu-id="e907f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="e907f-117">Các trang web dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết đúng.</span><span class="sxs-lookup"><span data-stu-id="e907f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
