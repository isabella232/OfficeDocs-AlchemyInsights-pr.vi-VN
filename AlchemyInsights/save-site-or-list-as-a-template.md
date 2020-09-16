---
title: Lưu site hoặc danh sách dưới dạng mẫu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727553"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="b5ede-102">Lưu site hoặc danh sách dưới dạng mẫu</span><span class="sxs-lookup"><span data-stu-id="b5ede-102">Save site or list as a template</span></span>

<span data-ttu-id="b5ede-103">Các mẫu site SharePoint là các định nghĩa được thiết kế sẵn xung quanh một nhu cầu doanh nghiệp cụ thể.</span><span class="sxs-lookup"><span data-stu-id="b5ede-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="b5ede-104">Để biết thêm thông tin, hãy xem [sử dụng mẫu để tạo các loại site SharePoint khác nhau](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="b5ede-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="b5ede-105">Dưới đây là một số vấn đề/giải pháp thông thường liên quan đến việc lưu một trang hoặc danh sách dưới dạng mẫu trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b5ede-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="b5ede-106">**Nút lưu site/danh sách không sẵn dùng hoặc bị thiếu**.</span><span class="sxs-lookup"><span data-stu-id="b5ede-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="b5ede-107">Người quản trị sẽ cần cho phép các tập lệnh tùy chỉnh cho phép các tính năng mẫu.</span><span class="sxs-lookup"><span data-stu-id="b5ede-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="b5ede-108">Để biết các bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn các kịch bản tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b5ede-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="b5ede-109">Lệnh lưu dưới dạng mẫu không được hỗ trợ và có thể gây ra sự cố trên các trang sử dụng cơ sở hạ tầng phát hành SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="b5ede-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="b5ede-110">**Không tạo được mẫu site hoặc không hoạt động đúng cách**</span><span class="sxs-lookup"><span data-stu-id="b5ede-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="b5ede-111">Mẫu có thể bị thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="b5ede-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="b5ede-112">Nếu tính năng này không sẵn dùng để kích hoạt trong tuyển tập trang hiện tại, bạn không thể sử dụng mẫu site để tạo một site.</span><span class="sxs-lookup"><span data-stu-id="b5ede-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="b5ede-113">Kiểm tra xem liệu có bất kỳ danh sách hay thư viện vượt quá [giới hạn dạng xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) của các mục 5000 khi điều này có thể chặn việc tạo một mẫu site hay không.</span><span class="sxs-lookup"><span data-stu-id="b5ede-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="b5ede-114">Site có thể đang sử dụng quá nhiều tài nguyên và do đó mẫu site vượt quá giới hạn megabyte (MB) 50.</span><span class="sxs-lookup"><span data-stu-id="b5ede-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="b5ede-115">Có sự cố khi hiển thị dữ liệu từ danh sách sử dụng cột tra cứu.</span><span class="sxs-lookup"><span data-stu-id="b5ede-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="b5ede-116">Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tra cứu chính xác trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="b5ede-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="b5ede-117">Để biết thêm thông tin chi tiết về các sự cố và giải pháp thông thường, vui lòng tham khảo, [tạo và sử dụng mẫu site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="b5ede-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

