---
title: Tạo site trong SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732304"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="07a46-102">Tạo các trang SharePoint bằng mẫu</span><span class="sxs-lookup"><span data-stu-id="07a46-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="07a46-103">Khả năng lưu site dưới dạng mẫu không được hỗ trợ với liên lạc hiện đại hoặc các site nhóm.</span><span class="sxs-lookup"><span data-stu-id="07a46-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="07a46-104">Để biết thêm thông tin về cách sử dụng mẫu [, hãy tải xuống và tải lên một site SharePoint dưới dạng mẫu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="07a46-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="07a46-105">Dưới đây là một số vấn đề/giải pháp thông thường liên quan đến việc lưu một trang hoặc danh sách dưới dạng mẫu trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="07a46-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="07a46-106">**Nút lưu site/danh sách không sẵn dùng hoặc bị thiếu**</span><span class="sxs-lookup"><span data-stu-id="07a46-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="07a46-107">Người quản trị sẽ cần cho phép các tập lệnh tùy chỉnh cho phép các tính năng mẫu.</span><span class="sxs-lookup"><span data-stu-id="07a46-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="07a46-108">Để biết các bước chi tiết, ví dụ và cân nhắc</span><span class="sxs-lookup"><span data-stu-id="07a46-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="07a46-109">Cho phép hoặc ngăn chặn các tập lệnh tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="07a46-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="07a46-110">Lệnh lưu dưới dạng mẫu không được hỗ trợ và có thể gây ra sự cố trên các trang sử dụng cơ sở hạ tầng phát hành SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="07a46-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="07a46-111">**Không tạo được mẫu site hoặc không hoạt động đúng cách**</span><span class="sxs-lookup"><span data-stu-id="07a46-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="07a46-112">Mẫu có thể bị thiếu một [tính năng](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) và sẽ không kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="07a46-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="07a46-113">Nếu tính năng này không sẵn dùng để kích hoạt trong tuyển tập trang hiện tại, bạn không thể sử dụng mẫu site để tạo một site.</span><span class="sxs-lookup"><span data-stu-id="07a46-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="07a46-114">Kiểm tra xem liệu có bất kỳ danh sách hay thư viện vượt quá [giới hạn dạng xem danh sách](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) của các mục 5000 khi điều này có thể chặn việc tạo một mẫu site hay không.</span><span class="sxs-lookup"><span data-stu-id="07a46-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="07a46-115">Site có thể đang sử dụng quá nhiều tài nguyên và do đó mẫu site vượt quá giới hạn 50 MB.</span><span class="sxs-lookup"><span data-stu-id="07a46-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="07a46-116">Có sự cố khi hiển thị dữ liệu từ danh sách sử dụng cột tra cứu.</span><span class="sxs-lookup"><span data-stu-id="07a46-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="07a46-117">Để biết thêm thông tin, hãy xem [danh sách tạo mẫu không hiển thị dữ liệu từ danh sách tra cứu chính xác trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="07a46-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="07a46-118">Để biết thêm thông tin chi tiết về các sự cố và giải pháp phổ biến, vui lòng kiểm tra [tạo và sử dụng mẫu site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="07a46-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



