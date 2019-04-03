---
title: Lưu trang web hoặc danh sách như là một bản mẫu
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044026"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="4c9b7-102">Lưu trang web hoặc danh sách như là một bản mẫu</span><span class="sxs-lookup"><span data-stu-id="4c9b7-102">Save site or list as a template</span></span>

<span data-ttu-id="4c9b7-103">SharePoint trang web mẫu là dựng sẵn định nghĩa được thiết kế quanh một nhu cầu doanh nghiệp cụ thể.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="4c9b7-104">Để biết thêm chi tiết, hãy xem [sử dụng mẫu để tạo ra các loại khác nhau của các trang web SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="4c9b7-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="4c9b7-105">Dưới đây là một số vấn đề phổ biến/giải pháp liên quan đến tiết kiệm một trang web hoặc danh sách như là một bản mẫu trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="4c9b7-106">**Lưu danh sách, trang web mẫu nút là không có sẵn hoặc mất tích**.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="4c9b7-107">Quản trị viên sẽ cần phải cho phép tuỳ chỉnh Script để kích hoạt tính năng mẫu.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="4c9b7-108">Bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4c9b7-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="4c9b7-109">Các trang web lưu như mẫu lệnh không được hỗ trợ và có thể gây ra vấn đề trên các trang web sử dụng các SharePoint Server xuất bản cơ sở hạ tầng.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


**<span data-ttu-id="4c9b7-110">Các mẫu trang web không thể được tạo ra hoặc không làm việc một cách chính xác</span><span class="sxs-lookup"><span data-stu-id="4c9b7-110">The site template cannot be created or does not work correctly</span></span>**

- <span data-ttu-id="4c9b7-111">Các mẫu có thể mất một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="4c9b7-112">Nếu các tính năng không có sẵn để kích hoạt trong bộ sưu tập trang web hiện tại, bạn không thể sử dụng các mẫu trang web để tạo ra một trang web.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="4c9b7-113">Kiểm tra xem nếu bất kỳ danh sách hoặc thư viện vượt quá [Danh sách nhìn giới hạn ngưỡng](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 mặt hàng như điều này có thể chặn các sáng tạo của một trang web mẫu.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="4c9b7-114">Các trang web có thể sử dụng quá nhiều tài nguyên, và do đó các mẫu trang web vượt quá giới hạn 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="4c9b7-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="4c9b7-115">Không có vấn đề Hiển thị các dữ liệu từ một danh sách mà sử dụng một cột tra cứu.</span><span class="sxs-lookup"><span data-stu-id="4c9b7-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="4c9b7-116">Để biết thêm chi tiết, hãy xem [tạo mẫu danh sách không hiển thị các dữ liệu từ danh sách tra cứu chính xác trong SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="4c9b7-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="4c9b7-117">Các thông tin chi tiết hơn về vấn đề thường gặp và các giải pháp, xin vui lòng tham khảo, [tạo và sử dụng các mẫu trang web](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="4c9b7-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

