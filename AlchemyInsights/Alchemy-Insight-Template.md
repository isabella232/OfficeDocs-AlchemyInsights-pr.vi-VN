---
title: giống như tên tập tin là tốt nhất
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750992"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="6bc1a-102">"Yêu cầu Alchemy header H1, H2's không làm việc."</span><span class="sxs-lookup"><span data-stu-id="6bc1a-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="6bc1a-103">Thực tiễn tốt nhất và hướng dẫn cho Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="6bc1a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="6bc1a-104">Không **làm tổ các hiểu biết Alchemy trong thư mục**-điều này sẽ phá vỡ cấu trúc URL.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="6bc1a-105">Chúng tôi đang tìm kiếm vào sửa chữa này.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="6bc1a-106">Các tệp trong thư mục **AlchemyInsights** nên có tên tập tin chữ thường với dấu gạch ngang cho không gian ex.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="6bc1a-107">***làm thế nào để kích hoạt-tranh chấp giữ***.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="6bc1a-108">Bao gồm ID quy tắc hoặc ID nhóm từ [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) trong trường MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="6bc1a-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-109">ex.</span></span> <span data-ttu-id="6bc1a-110">***MS. tùy chỉnh: 100021***</span><span class="sxs-lookup"><span data-stu-id="6bc1a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="6bc1a-111">Sử dụng phần còn lại của siêu dữ liệu ở đầu tệp này làm mẫu của bạn.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="6bc1a-112">Trong [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net), điều hướng xuống mục **khách hàng Insight tiêu đề:** và sử dụng đó như là một điểm khởi đầu cho tiêu đề H1 của bạn cho cái nhìn sâu sắc.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="6bc1a-113">Alchemy Insights phải có chỉ có một H1 duy nhất ở đầu hoặc họ sẽ phá vỡ trong sản xuất.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="6bc1a-114">H2s không hiển thị hoặc để sử dụng **đậm** hoặc các quy ước khác để biểu thị các phần riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="6bc1a-115">Tiếp theo, điền vào nội dung văn bản bằng cách sử dụng tài liệu dự thảo trong phần hiểu biết khách hàng của trang quy tắc giả kim thuật</span><span class="sxs-lookup"><span data-stu-id="6bc1a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="6bc1a-116">Danh sách có dấu đầu dòng là tốt</span><span class="sxs-lookup"><span data-stu-id="6bc1a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="6bc1a-117">Danh sách số quá</span><span class="sxs-lookup"><span data-stu-id="6bc1a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="6bc1a-118">**Bold** và *nghiêng* là một OK</span><span class="sxs-lookup"><span data-stu-id="6bc1a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="6bc1a-119">Liên kết phải luôn là **"liên kết đến web"/bên ngoài** hoặc **Deep-liên kết đến các yếu tố giao diện người dùng**, không liên kết nội bộ.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="6bc1a-120">Hình ảnh không được hỗ trợ chính thức vào thời gian này, nhưng nó trên lộ trình.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="6bc1a-121">Và điều này thực sự là đã có một chút quá dài.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="6bc1a-122">Thực hành tốt nhất là khoảng 400 ký tự---------------------------------</span><span class="sxs-lookup"><span data-stu-id="6bc1a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="6bc1a-123">Sau khi nội dung của bạn đã sẵn sàng, hãy kéo nó đến chi nhánh trực tiếp.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="6bc1a-124">Sau đó, đi đến [cổng thông tin đối tác giả kim](https://alchemyportal.azurewebsites.net) và nhập tên tệp vào trường URL.</span><span class="sxs-lookup"><span data-stu-id="6bc1a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 