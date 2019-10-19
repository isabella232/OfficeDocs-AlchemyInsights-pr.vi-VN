---
title: Hoán đổi trang web gốc cổ điển của bạn với một trang web hiện đại
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749282"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="1f2c5-102">Hoán đổi trang web gốc cổ điển của bạn với một trang web hiện đại</span><span class="sxs-lookup"><span data-stu-id="1f2c5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="1f2c5-103">Nếu môi trường của bạn đã được thiết lập trước ngày 2019, bạn có thể thay đổi trang web gốc của bạn sang một trang web hiện đại bằng cách sử dụng Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1f2c5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="1f2c5-104">Nếu bạn có một trang web khác mà bạn muốn sử dụng làm trang web gốc của bạn, bạn có thể thay thế [(Swap) các trang web gốc](https://docs.microsoft.com/sharepoint/modern-root-site) với nó.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="1f2c5-105">Sử dụng [gọi SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web trong khi lưu trữ các trang web ban đầu.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1f2c5-106">Có sẵn cho cả hai trang web nhóm (không được kết nối với một nhóm) và trang web truyền thông.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="1f2c5-107">Khả năng bổ sung sẽ được giới thiệu sớm mà sẽ cho phép bạn tiếp tục sử dụng các nội dung trên trang web, nhưng chuyển đổi các trang web hiện có đến một trang web liên lạc.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="1f2c5-108">Những khả năng này sẽ được cuộn dần.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="1f2c5-109">Tiếp tục kiểm tra Office 365 Message Center để cập nhật.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1f2c5-110">Các vấn đề với trao đổi trang web</span><span class="sxs-lookup"><span data-stu-id="1f2c5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="1f2c5-111">Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1f2c5-112">Nội dung cần phải được thu thập lại để cập nhật chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1f2c5-113">Không có hướng dẫn sử dụng bước cần thiết-điều này sẽ được thực hiện tự động.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="1f2c5-114">Bất cứ điều gì phụ thuộc vào "tĩnh" liên kết (chẳng hạn như tập tin Sync và OneNote tập tin) sẽ cần phải được sửa chữa thủ công.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1f2c5-115">Nếu trang web nguồn là một trang web tin tức tổ chức, Cập Nhật URL.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="1f2c5-116">Nhận danh sách tất cả các trang web tin tức tổ chức.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="1f2c5-117">Trang web máy chủ dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết chính xác.</span><span class="sxs-lookup"><span data-stu-id="1f2c5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





