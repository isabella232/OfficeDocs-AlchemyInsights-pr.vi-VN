---
title: Tạo một trang web trong SharePoint trực tuyến
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755330"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="2e2ed-102">Tạo các trang web SharePoint bằng cách sử dụng mẫu</span><span class="sxs-lookup"><span data-stu-id="2e2ed-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="2e2ed-103">Mẫu trang web SharePoint được xây dựng sẵn định nghĩa được thiết kế xung quanh một nhu cần kinh doanh cụ thể.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="2e2ed-104">Để biết thêm thông tin, xem [sử dụng mẫu để tạo các loại trang web SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="2e2ed-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="2e2ed-105">Dưới đây là một số vấn đề thường gặp/giải pháp liên quan đến lưu một trang web hoặc danh sách như một mẫu trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="2e2ed-106">**Lưu trang web/danh sách mẫu nút không có sẵn hoặc thiếu**</span><span class="sxs-lookup"><span data-stu-id="2e2ed-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="2e2ed-107">Quản trị viên sẽ cần cho phép tuỳ chỉnh script để kích hoạt các tính năng mẫu.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="2e2ed-108">Để biết các bước chi tiết, ví dụ và xem xét</span><span class="sxs-lookup"><span data-stu-id="2e2ed-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="2e2ed-109">Cho phép hoặc ngăn chặn tập lệnh tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="2e2ed-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="2e2ed-110">Lưu trang web dưới dạng lệnh không được hỗ trợ và có thể gây ra sự cố trên các trang web sử dụng SharePoint Server xuất bản cơ sở hạ tầng.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="2e2ed-111">**Mẫu trang web không thể tạo hoặc không hoạt động bình thường**</span><span class="sxs-lookup"><span data-stu-id="2e2ed-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="2e2ed-112">Mẫu có thể thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="2e2ed-113">Nếu tính năng không có sẵn để kích hoạt trong bộ sưu tập trang web hiện tại, bạn không thể sử dụng mẫu trang web để tạo một trang web.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="2e2ed-114">Kiểm tra xem nếu có danh sách hoặc thư viện vượt quá [ngưỡng giới hạn xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 mục vì điều này có thể chặn tạo một mẫu trang web.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="2e2ed-115">Trang web có thể sử dụng quá nhiều tài nguyên và do đó các trang web mẫu vượt quá giới hạn 50 MB.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="2e2ed-116">Có vấn đề Hiển thị dữ liệu từ danh sách sử dụng cột tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="2e2ed-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="2e2ed-117">Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tìm kiếm chính xác trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="2e2ed-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="2e2ed-118">Để biết thêm thông tin về các vấn đề và giải pháp phổ biến, hãy kiểm tra [tạo và sử dụng các mẫu trang web](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="2e2ed-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



