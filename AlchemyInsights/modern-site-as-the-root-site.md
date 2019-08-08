---
title: Các trang web hiện đại như các trang web gốc
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232737"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0544b-102">Các trang web hiện đại như là trang web gốc</span><span class="sxs-lookup"><span data-stu-id="0544b-102">Modern site as root site</span></span>

<span data-ttu-id="0544b-103">Chúng tôi đã bắt đầu buổi giới thiệu một tính năng mới mà sẽ cho phép bạn để hoán đổi cổ điển trang web trang web gốc của bạn với một trang web hiện đại.</span><span class="sxs-lookup"><span data-stu-id="0544b-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="0544b-104">Sử dụng [Gọi SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để trao đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang web gốc.</span><span class="sxs-lookup"><span data-stu-id="0544b-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="0544b-105">Sẵn sàng cho cả hai nhóm trang web (không kết nối với một nhóm) và trang web thông tin liên lạc.</span><span class="sxs-lookup"><span data-stu-id="0544b-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="0544b-106">Không xóa bỏ các trang web gốc cổ điển của bạn để tạo ra một trang web thông tin liên lạc hiện đại.</span><span class="sxs-lookup"><span data-stu-id="0544b-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0544b-107">Điều này không được hỗ trợ bởi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0544b-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="0544b-108">Xóa trang web gốc sẽ làm cho tất cả các trang web SharePoint trong tổ chức của bạn không thể tiếp cận tất cả người dùng, cho đến khi bạn khôi phục lại các trang web hoặc tạo một trang web mới tại cùng một URL.</span><span class="sxs-lookup"><span data-stu-id="0544b-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="0544b-109">Chúng tôi sẽ liên lạc các tính năng này thông qua Trung tâm tin nhắn.</span><span class="sxs-lookup"><span data-stu-id="0544b-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="0544b-110">Bạn có thể mong đợi các tính năng được bật trong người thuê nhà của bạn ngay.</span><span class="sxs-lookup"><span data-stu-id="0544b-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="0544b-111">Các vấn đề được biết đến với các trang web trao đổi</span><span class="sxs-lookup"><span data-stu-id="0544b-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="0544b-112">Trang web mục tiêu có thể trả lại một lỗi "không tìm thấy" (HTTP 404) cho một khoảng thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="0544b-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="0544b-113">Nội dung sẽ cần phải được recrawled để cập nhật danh mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="0544b-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="0544b-114">Không không có bước hướng dẫn sử dụng yêu cầu ở đây, điều này sẽ được thực hiện tự động.</span><span class="sxs-lookup"><span data-stu-id="0544b-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="0544b-115">Bất cứ điều gì phụ thuộc vào các liên kết "tĩnh" (chẳng hạn như đồng bộ hóa tập tin và OneNote files) sẽ cần phải được sửa chữa bằng tay.</span><span class="sxs-lookup"><span data-stu-id="0544b-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="0544b-116">Dự án máy chủ trang web có thể cần phải được xác nhận để đảm bảo rằng họ vẫn còn liên kết một cách chính xác.</span><span class="sxs-lookup"><span data-stu-id="0544b-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
