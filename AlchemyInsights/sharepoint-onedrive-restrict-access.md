---
title: Hạn chế quyền truy cập trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053787"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="6c977-102">Hạn chế quyền truy cập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="6c977-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="6c977-103">Có nhiều cách để hạn chế quyền truy cập vào dịch vụ SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6c977-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="6c977-104">Các phương pháp hạn chế truy cập khác nhau được nêu dưới đây.</span><span class="sxs-lookup"><span data-stu-id="6c977-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="6c977-105">**Hạn chế quyền**</span><span class="sxs-lookup"><span data-stu-id="6c977-105">**Permission Restriction**</span></span>

<span data-ttu-id="6c977-106">Trong SharePoint Online và OneDrive for Business, chúng tôi giới hạn quyền truy cập vào các mục như trang web, tệp và thư mục bằng cách chỉ cấp quyền truy cập vào các nhóm/cá nhân có quyền truy cập.</span><span class="sxs-lookup"><span data-stu-id="6c977-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="6c977-107">Tuỳ chỉnh quyền cho một danh sách SharePoint hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="6c977-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="6c977-108">Tùy chỉnh quyền trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="6c977-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="6c977-109">Thay đổi quyền trên một thư mục con</span><span class="sxs-lookup"><span data-stu-id="6c977-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="6c977-110">Kiểm soát truy cập từ các thiết bị không quản lý</span><span class="sxs-lookup"><span data-stu-id="6c977-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="6c977-111">Là một SharePoint hoặc quản trị toàn cầu trong Office 365, bạn có thể chặn hoặc giới hạn truy cập vào SharePoint và OneDrive nội dung từ thiết bị không được quản lý (những người không kết hợp AD tham gia hoặc phù hợp trong InTune).</span><span class="sxs-lookup"><span data-stu-id="6c977-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="6c977-112">**Giới hạn vị trí mạng**</span><span class="sxs-lookup"><span data-stu-id="6c977-112">**Network Location Restriction**</span></span>

<span data-ttu-id="6c977-113">Là quản trị viên CNTT, bạn có thể kiểm soát quyền truy cập vào tài nguyên SharePoint và OneDrive dựa trên các vị trí mạng được xác định mà bạn tin cậy.</span><span class="sxs-lookup"><span data-stu-id="6c977-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="6c977-114">Điều này còn được gọi là chính sách dựa trên vị trí.</span><span class="sxs-lookup"><span data-stu-id="6c977-114">This is also known as location-based policy.</span></span> <span data-ttu-id="6c977-115">Để biết thêm thông tin, hãy xem [kiểm soát truy cập vào dữ liệu SharePoint trực tuyến và OneDrive dựa trên vị trí mạng](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="6c977-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="6c977-116">**Hạn chế khóa trang web**</span><span class="sxs-lookup"><span data-stu-id="6c977-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="6c977-117">Trong SharePoint Online, bạn có khả năng khóa một bộ sưu tập trang web, do đó, không ai có quyền truy cập.</span><span class="sxs-lookup"><span data-stu-id="6c977-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="6c977-118">Điều này được thiết lập qua PowerShell và [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng cách sử dụng thuộc tính [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="6c977-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="6c977-119">**Hạn chế người dùng tạo trang web hoặc trang web con**</span><span class="sxs-lookup"><span data-stu-id="6c977-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="6c977-120">Là một quản trị SharePoint hoặc quản trị viên toàn cầu Office 365, bạn có thể cho phép người dùng của bạn tạo và quản lý các trang web SharePoint của riêng họ, xác định loại trang web mà họ có thể tạo và chỉ định vị trí của các trang web.</span><span class="sxs-lookup"><span data-stu-id="6c977-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="6c977-121">Để biết thêm thông tin, hãy xem [quản lý tạo trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="6c977-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

