---
title: Hạn chế truy cập trong SharePoint hoặc OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223734"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="6dc54-102">Hạn chế truy cập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="6dc54-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="6dc54-103">Có rất nhiều cách để hạn chế truy cập vào các dịch vụ SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6dc54-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="6dc54-104">Những phương pháp hạn chế truy cập khác nhau được trình bày dưới đây.</span><span class="sxs-lookup"><span data-stu-id="6dc54-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="6dc54-105">**Quyền hạn chế**</span><span class="sxs-lookup"><span data-stu-id="6dc54-105">**Permission Restriction**</span></span>

<span data-ttu-id="6dc54-106">Trong trực tuyến SharePoint và OneDrive cho doanh nghiệp, chúng tôi giới hạn truy cập vào các mục như các trang web, tập tin và thư mục bằng cách chỉ cấp quyền truy cập vào các nhóm/cá nhân nên có thể truy cập.</span><span class="sxs-lookup"><span data-stu-id="6dc54-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="6dc54-107">Tùy chỉnh cấp phép cho một danh sách SharePoint hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="6dc54-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="6dc54-108">Tùy chỉnh cho phép trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="6dc54-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="6dc54-109">Thay đổi quyền truy cập vào một thư mục con</span><span class="sxs-lookup"><span data-stu-id="6dc54-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="6dc54-110">Điều khiển truy cập từ các thiết bị không được quản lý</span><span class="sxs-lookup"><span data-stu-id="6dc54-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="6dc54-111">SharePoint hoặc quản trị toàn cầu trong Office 365, bạn có thể chặn hoặc hạn chế quyền truy cập vào nội dung SharePoint và OneDrive từ các thiết bị không được quản lý (những người không kết hợp quảng cáo tham gia hoặc tuân thủ trong dành).</span><span class="sxs-lookup"><span data-stu-id="6dc54-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="6dc54-112">**Giới hạn vị trí mạng**</span><span class="sxs-lookup"><span data-stu-id="6dc54-112">**Network Location Restriction**</span></span>

<span data-ttu-id="6dc54-113">Như là quản trị viên CNTT, bạn có thể kiểm soát quyền truy cập vào tài nguyên SharePoint và OneDrive dựa trên vị trí xác định mạng mà bạn tin tưởng.</span><span class="sxs-lookup"><span data-stu-id="6dc54-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="6dc54-114">Điều này cũng được gọi là chính sách dựa trên vị trí.</span><span class="sxs-lookup"><span data-stu-id="6dc54-114">This is also known as location-based policy.</span></span> <span data-ttu-id="6dc54-115">Để biết thêm chi tiết, xin vui lòng xem [kiểm soát quyền truy cập vào dữ liệu OneDrive dựa trên vị trí mạng và SharePoint Online](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="6dc54-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="6dc54-116">**Trang web Lock hạn chế**</span><span class="sxs-lookup"><span data-stu-id="6dc54-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="6dc54-117">Trong SharePoint Online, bạn có khả năng khóa xuống một bộ sưu tập trang web, do đó, không ai có quyền truy cập.</span><span class="sxs-lookup"><span data-stu-id="6dc54-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="6dc54-118">Điều này được thiết lập qua PowerShell và [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng cách sử dụng [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState tài sản.</span><span class="sxs-lookup"><span data-stu-id="6dc54-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="6dc54-119">**Hạn chế người dùng từ việc tạo ra trang web này hoặc SubSite**</span><span class="sxs-lookup"><span data-stu-id="6dc54-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="6dc54-120">Như là một quản trị SharePoint hoặc Office 365 quản trị toàn cầu, bạn có thể cho phép người dùng tạo và quản lý các trang web SharePoint của riêng họ, xác định những loại trang web, họ có thể tạo ra, và xác định vị trí các trang web.</span><span class="sxs-lookup"><span data-stu-id="6dc54-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="6dc54-121">Để biết thêm chi tiết, hãy xem [quản lý tạo ra trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="6dc54-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

