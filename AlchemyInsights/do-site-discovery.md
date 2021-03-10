---
title: Thực hiện khám phá trang
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694552"
---
# <a name="do-site-discovery"></a><span data-ttu-id="f76b7-102">Thực hiện khám phá trang</span><span class="sxs-lookup"><span data-stu-id="f76b7-102">Do site discovery</span></span>

<span data-ttu-id="f76b7-103">Nếu tổ chức của bạn vẫn sử dụng các ứng dụng web kế thừa và các gói sử dụng chế độ Internet Explorer (mà hầu hết khách hàng thực hiện), thì bạn nên thực hiện một số khám phá trang bổ sung.</span><span class="sxs-lookup"><span data-stu-id="f76b7-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="f76b7-104">**Bạn đã triển khai phiên bản Microsoft Edge cũ hơn**</span><span class="sxs-lookup"><span data-stu-id="f76b7-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="f76b7-105">Nếu bạn đã cấu hình danh sách trang web doanh nghiệp của bạn để làm việc cho phiên bản kế thừa của Microsoft Edge, sau đó phát hiện trang web của bạn gần như đã hoàn tất.</span><span class="sxs-lookup"><span data-stu-id="f76b7-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="f76b7-106">Một trong những điều bạn có thể cần làm là thêm site trung lập.</span><span class="sxs-lookup"><span data-stu-id="f76b7-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="f76b7-107">Site trung bình thường là các site cung cấp đăng nhập đơn (SSO).</span><span class="sxs-lookup"><span data-stu-id="f76b7-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="f76b7-108">Nếu bạn đi đến một site trung lập từ Microsoft Edge, thì bạn muốn ở trong Microsoft Edge để xác thực.</span><span class="sxs-lookup"><span data-stu-id="f76b7-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="f76b7-109">Nếu bạn đi đến một site trung lập trong chế độ Internet Explorer, thì bạn muốn giữ lại trong chế độ Internet Explorer để xác thực.</span><span class="sxs-lookup"><span data-stu-id="f76b7-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="f76b7-110">Xác định bất kỳ SSO hoặc các site trung lập nào mà bạn sử dụng và thêm vào danh sách trang web doanh nghiệp của bạn.</span><span class="sxs-lookup"><span data-stu-id="f76b7-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="f76b7-111">**Internet Explorer là trình duyệt mặc định của bạn**</span><span class="sxs-lookup"><span data-stu-id="f76b7-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="f76b7-112">Nếu bạn chỉ đang dùng Internet Explorer, bạn có thể không biết site nào đã nâng cấp lên tiêu chuẩn web hiện đại và vẫn yêu cầu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f76b7-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="f76b7-113">Bạn sẽ muốn tìm và thêm các site này vào danh sách site của doanh nghiệp để bạn có thể sử dụng chế độ Internet Explorer cho các site đó.</span><span class="sxs-lookup"><span data-stu-id="f76b7-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="f76b7-114">[Khám phá trang Enterprise phát hiện](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) ra các site có thể cần chế độ Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f76b7-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="f76b7-115">Ứng dụng này có thể thu thập dữ liệu trên các máy tính chạy Windows Internet Explorer 8 thông qua Internet Explorer 11 trên Windows 10, Windows 8,1 hoặc Windows 7.</span><span class="sxs-lookup"><span data-stu-id="f76b7-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="f76b7-116">**Phân tích dữ liệu**</span><span class="sxs-lookup"><span data-stu-id="f76b7-116">**Analyze the data**</span></span>

<span data-ttu-id="f76b7-117">Sau khi bạn đã thu thập dữ liệu site, chúng tôi khuyên bạn nên quy trình bốn bước sau đây để phân tích dữ liệu:</span><span class="sxs-lookup"><span data-stu-id="f76b7-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="f76b7-118">Sắp xếp dữ liệu theo tên miền, rồi theo URL.</span><span class="sxs-lookup"><span data-stu-id="f76b7-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="f76b7-119">Xác định ranh giới của một ứng dụng để cấu hình cho chế độ Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f76b7-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="f76b7-120">Bạn muốn bao gồm tất cả các site và điều khiển web xác định ứng dụng, nhưng bạn không muốn bao gồm các site và điều khiển bổ sung.</span><span class="sxs-lookup"><span data-stu-id="f76b7-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="f76b7-121">Một số site có thể đơn giản như *https://contoso.com/app1* trong khi những người khác có thể yêu cầu bạn xác định nhiều site và trang.</span><span class="sxs-lookup"><span data-stu-id="f76b7-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="f76b7-122">Kiểm tra ứng dụng để xác nhận rằng nó không hoạt động chính.</span><span class="sxs-lookup"><span data-stu-id="f76b7-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="f76b7-123">Nhiều site sẽ cung cấp nội dung hiện đại khi họ phát hiện ra một trình duyệt hiện đại và chỉ cung cấp nội dung kế thừa khi họ phát hiện Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f76b7-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="f76b7-124">Thêm ứng dụng vào danh sách site doanh nghiệp của bạn nếu nó không được kiểm tra.</span><span class="sxs-lookup"><span data-stu-id="f76b7-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="f76b7-125">Thực hành tốt nhất, nhóm tất cả các site có bao gồm một ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="f76b7-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="f76b7-126">Bằng cách này, khi bạn nâng cấp một ứng dụng, bạn sẽ dễ dàng loại bỏ toàn bộ site khỏi chế độ Internet Explorer và bắt đầu sử dụng trình duyệt hiện đại cho ứng dụng đó.</span><span class="sxs-lookup"><span data-stu-id="f76b7-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="f76b7-127">Sau khi bạn đã thực hiện xong với khám phá trang và bạn đã phân tích dữ liệu, bạn đã sẵn sàng để bắt đầu xem chiến lược kênh của mình.</span><span class="sxs-lookup"><span data-stu-id="f76b7-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

