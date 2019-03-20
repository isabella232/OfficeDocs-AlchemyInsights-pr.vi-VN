---
title: giống như tên tập tin là tốt nhất
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683871"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fe153-102">Yêu cầu Alchemy tiêu đề H1, H2 của không làm việc.</span><span class="sxs-lookup"><span data-stu-id="fe153-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="fe153-103">Thực hành và hướng dẫn cho tác giả kim thuật tốt nhất:</span><span class="sxs-lookup"><span data-stu-id="fe153-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fe153-104">**Không lồng Alchemy Insights trong thư mục này**- điều này sẽ phá vỡ cấu trúc url.</span><span class="sxs-lookup"><span data-stu-id="fe153-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fe153-105">Chúng tôi đang xem xét khắc phục điều này.</span><span class="sxs-lookup"><span data-stu-id="fe153-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fe153-106">Các tập tin trong thư mục **AlchemyInsights** cần phải có tên tập tin chữ thường với dấu gạch nối cho không gian ví dụ.</span><span class="sxs-lookup"><span data-stu-id="fe153-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fe153-107">***làm thế nào-to-enable--duy trì tranh chấp***.</span><span class="sxs-lookup"><span data-stu-id="fe153-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fe153-108">Bao gồm các quy tắc ID hoặc Xô ID từ [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) trong trường ms.custom.</span><span class="sxs-lookup"><span data-stu-id="fe153-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fe153-109">ex.</span><span class="sxs-lookup"><span data-stu-id="fe153-109">ex.</span></span> <span data-ttu-id="fe153-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="fe153-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fe153-111">Sử dụng phần còn lại của các siêu dữ liệu ở đầu file này như là bản mẫu của bạn.</span><span class="sxs-lookup"><span data-stu-id="fe153-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fe153-112">Trong các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net), di chuyển xuống mục **tiêu đề thấu hiểu khách hàng:** và sử dụng rằng, cũng như bắt đầu từ một điểm cho tiêu đề H1 của bạn cho sự thấu hiểu.</span><span class="sxs-lookup"><span data-stu-id="fe153-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fe153-113">Giả kim thuật Insights phải có chỉ một H1 đơn ở đầu trang hoặc họ sẽ phá vỡ trong sản xuất.</span><span class="sxs-lookup"><span data-stu-id="fe153-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fe153-114">H2s không hiển thị vì vậy sử dụng **đậm** hoặc các công ước để biểu thị phần riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="fe153-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fe153-115">Tiếp theo, điền vào trong cơ thể văn bản bằng cách sử dụng các tài liệu dự thảo trong phần hiểu biết khách hàng của trang giả kim thuật cai trị</span><span class="sxs-lookup"><span data-stu-id="fe153-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fe153-116">Danh sách dấu đầu dòng cũng tốt</span><span class="sxs-lookup"><span data-stu-id="fe153-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fe153-117">Đánh số các danh sách quá</span><span class="sxs-lookup"><span data-stu-id="fe153-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fe153-118">**Đậm** và *nghiêng* là a-ok</span><span class="sxs-lookup"><span data-stu-id="fe153-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fe153-119">Liên kết nên luôn luôn là một trong hai **"liên kết đến các trang web" / ngoài** OR **sâu-liên kết đến các yếu tố giao diện người dùng**, không phải nội bộ liên kết.</span><span class="sxs-lookup"><span data-stu-id="fe153-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fe153-120">Hình ảnh không hỗ trợ chính thức tại thời điểm này, nhưng nó là trên lộ trình.</span><span class="sxs-lookup"><span data-stu-id="fe153-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fe153-121">Và điều này thực sự đã là một chút quá dài.</span><span class="sxs-lookup"><span data-stu-id="fe153-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fe153-122">Thực hành tốt nhất là khoảng 400 ký tự---</span><span class="sxs-lookup"><span data-stu-id="fe153-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fe153-123">Khi nội dung của bạn đã sẵn sàng, kéo nó tới các chi nhánh trực tiếp.</span><span class="sxs-lookup"><span data-stu-id="fe153-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fe153-124">Sau đó, các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) và nhập tên tập tin vào trường url.</span><span class="sxs-lookup"><span data-stu-id="fe153-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="fe153-125">M</span><span class="sxs-lookup"><span data-stu-id="fe153-125">M</span></span>