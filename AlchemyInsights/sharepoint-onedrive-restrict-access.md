---
title: Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700477"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="03311-102">Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="03311-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="03311-103">Có nhiều cách để hạn chế quyền truy nhập vào các dịch vụ SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="03311-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="03311-104">Những phương pháp hạn chế truy nhập khác nhau được nêu dưới đây.</span><span class="sxs-lookup"><span data-stu-id="03311-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="03311-105">**Hạn chế cấp phép**</span><span class="sxs-lookup"><span data-stu-id="03311-105">**Permission Restriction**</span></span>

<span data-ttu-id="03311-106">Trong SharePoint Online và OneDrive for Business, chúng tôi giới hạn quyền truy nhập vào các mục như site, tệp và thư mục bằng cách chỉ cấp quyền truy nhập vào các nhóm/cá nhân cần có quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="03311-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="03311-107">Tùy chỉnh quyền đối với danh sách hoặc thư viện SharePoint</span><span class="sxs-lookup"><span data-stu-id="03311-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="03311-108">Tùy chỉnh quyền đối với site SharePoint</span><span class="sxs-lookup"><span data-stu-id="03311-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="03311-109">Thay đổi quyền trên thư mục con</span><span class="sxs-lookup"><span data-stu-id="03311-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="03311-110">Kiểm soát truy nhập từ thiết bị không được quản lý</span><span class="sxs-lookup"><span data-stu-id="03311-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="03311-111">Với tư cách là người quản trị SharePoint hoặc toàn cầu, bạn có thể chặn hoặc giới hạn quyền truy nhập vào SharePoint và OneDrive từ các thiết bị không được quản lý (không kết hợp với quảng cáo được gia nhập hoặc tuân thủ trong InTune).</span><span class="sxs-lookup"><span data-stu-id="03311-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="03311-112">**Giới hạn vị trí mạng**</span><span class="sxs-lookup"><span data-stu-id="03311-112">**Network Location Restriction**</span></span>

<span data-ttu-id="03311-113">Với tư cách là người quản trị CNTT, bạn có thể kiểm soát quyền truy nhập vào các tài nguyên SharePoint và OneDrive dựa trên vị trí mạng được xác định bạn tin tưởng.</span><span class="sxs-lookup"><span data-stu-id="03311-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="03311-114">Điều này còn được gọi là chính sách dựa trên vị trí.</span><span class="sxs-lookup"><span data-stu-id="03311-114">This is also known as location-based policy.</span></span> <span data-ttu-id="03311-115">Để biết thêm thông tin, vui lòng xem [kiểm soát quyền truy nhập vào dữ liệu SharePoint Online và OneDrive dựa trên vị trí mạng](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="03311-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="03311-116">**Giới hạn khóa của site**</span><span class="sxs-lookup"><span data-stu-id="03311-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="03311-117">Trong SharePoint Online, bạn có khả năng khóa một tuyển tập trang, vì vậy không ai có quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="03311-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="03311-118">Điều này được đặt thông qua PowerShell và [Shell quản lý SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng thuộc tính [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="03311-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="03311-119">**Hạn chế người dùng tạo site hoặc trang phụ**</span><span class="sxs-lookup"><span data-stu-id="03311-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="03311-120">Với tư cách là người quản trị SharePoint hoặc người quản trị toàn cầu, bạn có thể cho phép người dùng của mình tạo và quản lý các site SharePoint riêng của họ, xác định loại site nào mà họ có thể tạo và xác định vị trí của các site.</span><span class="sxs-lookup"><span data-stu-id="03311-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="03311-121">Để biết thêm thông tin, vui lòng xem [quản lý việc tạo site trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="03311-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

