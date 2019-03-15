---
title: 'tương tự như là tên tập tin là tốt nhất [RULE #-mô tả]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634526"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="9f8c0-102">Yêu cầu Alchemy tiêu đề H1, H2 của không làm việc.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="9f8c0-103">Thực hành và hướng dẫn cho tác giả kim thuật tốt nhất:</span><span class="sxs-lookup"><span data-stu-id="9f8c0-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="9f8c0-104">**Không lồng Alchemy Insights trong thư mục này**- điều này sẽ phá vỡ cấu trúc url.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="9f8c0-105">Chúng tôi đang xem xét khắc phục điều này.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="9f8c0-106">Các tập tin trong thư mục **AlchemyInsights** cần phải có quy tắc ID và tên quy tắc từ [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) trong tên tập tin.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="9f8c0-107">ex.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-107">ex.</span></span> <span data-ttu-id="9f8c0-108">***976-How-to-Enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="9f8c0-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="9f8c0-109">Sử dụng các siêu dữ liệu ở đầu file này như là bản mẫu của bạn.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="9f8c0-110">Không có gì khác là cần thiết.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-110">Nothing else is required.</span></span>
1. <span data-ttu-id="9f8c0-111">Trong các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net), di chuyển xuống mục **tiêu đề thấu hiểu khách hàng:** và sử dụng rằng, cũng như bắt đầu từ một điểm cho tiêu đề H1 của bạn cho sự thấu hiểu.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="9f8c0-112">Giả kim thuật Insights phải có chỉ một H1 đơn ở đầu trang hoặc họ sẽ phá vỡ trong sản xuất.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="9f8c0-113">H2s không hiển thị vì vậy sử dụng **đậm** hoặc các công ước để biểu thị phần riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="9f8c0-114">Tiếp theo, điền vào trong cơ thể văn bản bằng cách sử dụng các tài liệu dự thảo trong phần hiểu biết khách hàng của trang giả kim thuật cai trị</span><span class="sxs-lookup"><span data-stu-id="9f8c0-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="9f8c0-115">Danh sách dấu đầu dòng cũng tốt</span><span class="sxs-lookup"><span data-stu-id="9f8c0-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="9f8c0-116">Đánh số các danh sách quá</span><span class="sxs-lookup"><span data-stu-id="9f8c0-116">Numbered lists too</span></span>
    1. <span data-ttu-id="9f8c0-117">**Đậm** và *nghiêng* là a-ok</span><span class="sxs-lookup"><span data-stu-id="9f8c0-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="9f8c0-118">Liên kết nên luôn luôn là một trong hai **"liên kết đến các trang web" / ngoài** OR **sâu-liên kết đến các yếu tố giao diện người dùng**, không phải nội bộ liên kết.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="9f8c0-119">Và điều này thực sự đã là một chút quá dài.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-119">And this is really already a bit too long.</span></span> <span data-ttu-id="9f8c0-120">Thực hành tốt nhất là khoảng 400 ký tự---</span><span class="sxs-lookup"><span data-stu-id="9f8c0-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="9f8c0-121">Khi nội dung của bạn đã sẵn sàng, kéo nó tới các chi nhánh trực tiếp.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="9f8c0-122">Sau đó, các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) và nhập tên tập tin vào trường url.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="9f8c0-123">Đảm bảo rằng cái nhìn sâu sắc được nhận xét và công bố nói "có" và sau đó bấm vào Cập Nhật quy tắc.</span><span class="sxs-lookup"><span data-stu-id="9f8c0-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="9f8c0-124">**(Điều này sẽ nhìn đẹp hơn trong phiên bản mới của portal - phát hành sớm.)** 
 ![trường url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="9f8c0-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

