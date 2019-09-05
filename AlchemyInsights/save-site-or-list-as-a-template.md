---
title: Lưu trang web hoặc danh sách dưới dạng mẫu
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752054"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="4ebfb-102">Lưu trang web hoặc danh sách dưới dạng mẫu</span><span class="sxs-lookup"><span data-stu-id="4ebfb-102">Save site or list as a template</span></span>

<span data-ttu-id="4ebfb-103">Mẫu trang web SharePoint được xây dựng sẵn định nghĩa được thiết kế xung quanh một nhu cần kinh doanh cụ thể.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="4ebfb-104">Để biết thêm thông tin, xem [sử dụng mẫu để tạo các loại trang web SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="4ebfb-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="4ebfb-105">Dưới đây là một số vấn đề thường gặp/giải pháp liên quan đến lưu một trang web hoặc danh sách như một mẫu trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="4ebfb-106">**Lưu trang web/danh sách mẫu nút không có sẵn hoặc thiếu**.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="4ebfb-107">Quản trị viên sẽ cần cho phép tuỳ chỉnh script để kích hoạt các tính năng mẫu.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="4ebfb-108">Đối với các bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4ebfb-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="4ebfb-109">Lưu trang web dưới dạng lệnh không được hỗ trợ và có thể gây ra sự cố trên các trang web sử dụng SharePoint Server xuất bản cơ sở hạ tầng.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="4ebfb-110">**Mẫu trang web không thể tạo hoặc không hoạt động bình thường**</span><span class="sxs-lookup"><span data-stu-id="4ebfb-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="4ebfb-111">Mẫu có thể thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="4ebfb-112">Nếu tính năng không có sẵn để kích hoạt trong bộ sưu tập trang web hiện tại, bạn không thể sử dụng mẫu trang web để tạo một trang web.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="4ebfb-113">Kiểm tra xem nếu có danh sách hoặc thư viện vượt quá [ngưỡng giới hạn xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 mục vì điều này có thể chặn tạo một mẫu trang web.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="4ebfb-114">Trang web có thể sử dụng quá nhiều tài nguyên và do đó mẫu trang web vượt quá giới hạn 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="4ebfb-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="4ebfb-115">Có vấn đề Hiển thị dữ liệu từ danh sách sử dụng cột tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="4ebfb-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="4ebfb-116">Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tìm kiếm chính xác trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="4ebfb-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="4ebfb-117">Để biết thêm thông tin về các vấn đề và giải pháp phổ biến, vui lòng tham khảo, [tạo và sử dụng các mẫu trang web](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="4ebfb-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

