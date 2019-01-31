---
title: 'tương tự như là tên tập tin là tốt nhất [RULE #-mô tả]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662952"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="ec87d-102">Yêu cầu khách hàng phải đối mặt với H1, H2 không hoạt động</span><span class="sxs-lookup"><span data-stu-id="ec87d-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="ec87d-103">Ví dụ văn bản chặn - hãy làm theo các hướng dẫn sau:</span><span class="sxs-lookup"><span data-stu-id="ec87d-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="ec87d-104">Các tập tin trong thư mục **AlchemyInsights** cần phải có quy tắc ID và tên quy tắc từ [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) trong tên tập tin.</span><span class="sxs-lookup"><span data-stu-id="ec87d-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="ec87d-p101">Ví dụ: ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="ec87d-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="ec87d-p102">Sử dụng các siêu dữ liệu ở đầu file này như là bản mẫu của bạn. Không có gì khác là cần thiết.</span><span class="sxs-lookup"><span data-stu-id="ec87d-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="ec87d-109">Trong các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net), di chuyển xuống mục **tiêu đề thấu hiểu khách hàng:** và sử dụng rằng, cũng như bắt đầu từ một điểm cho tiêu đề H1 của bạn cho sự thấu hiểu.</span><span class="sxs-lookup"><span data-stu-id="ec87d-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ec87d-p103">Giả kim thuật Insights phải có chỉ một H1 đơn ở đầu trang hoặc họ sẽ phá vỡ trong sản xuất. H2s không hiển thị vì vậy sử dụng **đậm** hoặc các công ước để biểu thị phần riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="ec87d-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ec87d-112">Tiếp theo, điền vào trong cơ thể văn bản bằng cách sử dụng các tài liệu dự thảo trong phần hiểu biết khách hàng của trang giả kim thuật cai trị</span><span class="sxs-lookup"><span data-stu-id="ec87d-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ec87d-113">Danh sách dấu đầu dòng cũng tốt</span><span class="sxs-lookup"><span data-stu-id="ec87d-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ec87d-114">Đánh số các danh sách quá</span><span class="sxs-lookup"><span data-stu-id="ec87d-114">Numbered lists too</span></span>
    1. <span data-ttu-id="ec87d-115">**Đậm** và *nghiêng* là a-ok</span><span class="sxs-lookup"><span data-stu-id="ec87d-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ec87d-116">Liên kết nên luôn luôn là một trong hai **"liên kết đến các trang web" / ngoài** OR **sâu-liên kết đến các yếu tố giao diện người dùng**, không phải nội bộ liên kết.</span><span class="sxs-lookup"><span data-stu-id="ec87d-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="ec87d-p104">Và điều này thực sự đã là một chút quá dài. Thực hành tốt nhất là khoảng 400 ký tự---</span><span class="sxs-lookup"><span data-stu-id="ec87d-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ec87d-p105">Khi nội dung của bạn đã sẵn sàng, kéo nó tới các chi nhánh trực tiếp. Sau đó, các [cổng thông tin đối tác giả kim thuật](https://alchemyportal.azurewebsites.net) và nhập tên tập tin vào trường url. Đảm bảo rằng cái nhìn sâu sắc được nhận xét và công bố nói "có" và sau đó bấm vào Cập Nhật quy tắc. (Điều này sẽ nhìn đẹp hơn trong phiên bản mới của portal - phát hành sớm.)</span><span class="sxs-lookup"><span data-stu-id="ec87d-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL field](media/for-content-team.PNG)

