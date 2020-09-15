---
title: tương tự như tên tệp là tốt nhất
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664156"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="ed933-102">"H1 tiêu đề Alchemy bắt buộc, H2's không hoạt động."</span><span class="sxs-lookup"><span data-stu-id="ed933-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="ed933-103">Phương pháp tốt nhất và hướng dẫn cho tác giả Alchemy:</span><span class="sxs-lookup"><span data-stu-id="ed933-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="ed933-104">Không **làm tổ những cái nhìn giả kim thuật trong thư mục**-điều này sẽ ngắt cấu trúc URL.</span><span class="sxs-lookup"><span data-stu-id="ed933-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="ed933-105">Chúng tôi đang tìm cách khắc phục sự cố này.</span><span class="sxs-lookup"><span data-stu-id="ed933-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="ed933-106">Các tệp trong thư mục **Alchemyinsights** cần có tên tệp chữ thường với dấu gạch nối cho các dấu cách cũ.</span><span class="sxs-lookup"><span data-stu-id="ed933-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="ed933-107">***làm thế nào để kích hoạt-giữ tranh chấp***.</span><span class="sxs-lookup"><span data-stu-id="ed933-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="ed933-108">Đưa vào ID quy tắc hoặc ID Xô từ [cổng thông tin đối tác Alchemy](https://alchemyportal.azurewebsites.net) trong trường MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="ed933-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="ed933-109">OKB.</span><span class="sxs-lookup"><span data-stu-id="ed933-109">ex.</span></span> <span data-ttu-id="ed933-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="ed933-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="ed933-111">Sử dụng phần còn lại của siêu dữ liệu ở phía trên cùng của tệp này làm mẫu của bạn.</span><span class="sxs-lookup"><span data-stu-id="ed933-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="ed933-112">Trong [cổng thông tin đối tác Alchemy](https://alchemyportal.azurewebsites.net), dẫn hướng xuống đến **tiêu đề của khách hàng phần Insight:** và sử dụng làm điểm bắt đầu cho tiêu đề H1 của bạn cho cái nhìn sâu sắc.</span><span class="sxs-lookup"><span data-stu-id="ed933-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ed933-113">Những cái nhìn giả kim thuật phải chỉ có một H1 duy nhất ở trên cùng hoặc chúng sẽ ngắt trong sản xuất.</span><span class="sxs-lookup"><span data-stu-id="ed933-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="ed933-114">H2s không khiến cho việc sử dụng các công ước **đậm** hoặc khác để biểu thị các phần riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="ed933-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ed933-115">Tiếp theo, điền vào nội dung văn bản bằng cách sử dụng tài liệu dự thảo trong phần Insights của khách hàng của trang quy tắc Alchemy</span><span class="sxs-lookup"><span data-stu-id="ed933-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ed933-116">Danh sách dấu đầu dòng là tốt</span><span class="sxs-lookup"><span data-stu-id="ed933-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ed933-117">Danh sách đánh số quá</span><span class="sxs-lookup"><span data-stu-id="ed933-117">Numbered lists too</span></span>
    1. <span data-ttu-id="ed933-118">**Đậm** và *nghiêng* là một OK</span><span class="sxs-lookup"><span data-stu-id="ed933-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ed933-119">Liên kết luôn phải là **"nối kết đến web"/bên ngoài** hoặc **liên kết sâu đến các thành phần giao diện người dùng**, không liên kết nội bộ.</span><span class="sxs-lookup"><span data-stu-id="ed933-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="ed933-120">Ảnh không được hỗ trợ chính thức vào thời điểm này, nhưng trên lộ trình.</span><span class="sxs-lookup"><span data-stu-id="ed933-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="ed933-121">Và điều này thực sự là một chút quá dài.</span><span class="sxs-lookup"><span data-stu-id="ed933-121">And this is really already a bit too long.</span></span> <span data-ttu-id="ed933-122">Cách thực hành tốt nhất là giới thiệu về 400---------------------------------</span><span class="sxs-lookup"><span data-stu-id="ed933-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ed933-123">Sau khi nội dung của bạn đã sẵn sàng, hãy kéo nó đến chi nhánh trực tiếp.</span><span class="sxs-lookup"><span data-stu-id="ed933-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="ed933-124">Sau đó, đi đến [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) và nhập tên tệp vào trường URL.</span><span class="sxs-lookup"><span data-stu-id="ed933-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 