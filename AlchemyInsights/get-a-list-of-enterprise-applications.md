---
title: Lấy danh sách các ứng dụng doanh nghiệp
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405507"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="c54d2-102">Lấy danh sách các ứng dụng doanh nghiệp</span><span class="sxs-lookup"><span data-stu-id="c54d2-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="c54d2-103">Để **lấy danh sách các ứng dụng doanh nghiệp** (Tất cả các ứng dụng hoặc được lọc theo tên hiển thị, ID, mã định danh Uris, v.v.) thông qua lệnh PowerShell, hãy xem [Get-AzureADApplication (azuread)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="c54d2-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="c54d2-104">Để lấy danh sách các đối tượng chính của dịch vụ (Tất cả đối tượng hoặc lọc theo ID) thông qua lệnh PowerShell, hãy xem [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="c54d2-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="c54d2-105">Nếu bạn muốn **lấy danh sách các ứng dụng được cấu hình SAML, sau đây là các script PowerShell** có thể giúp bạn:</span><span class="sxs-lookup"><span data-stu-id="c54d2-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="c54d2-106">Mỗi ứng dụng có thể là ứng dụng OAuth hoặc SAML (cả bộ sưu tập và ứng dụng không phải là bộ sưu tập) sẽ có hai đối tượng được tạo ra trong khi đăng ký của họ sẽ xảy ra.</span><span class="sxs-lookup"><span data-stu-id="c54d2-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="c54d2-107">Một được gọi là đối tượng ứng dụng và đó là đối tượng dịch vụ chính.</span><span class="sxs-lookup"><span data-stu-id="c54d2-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="c54d2-108">Khi bạn đổ các thuộc tính của một đối tượng dịch vụ chủ yếu bằng cách sử dụng PowerShell, bạn sẽ thấy rằng mọi ứng dụng đều có một số lượng thẻ nhất định được liên kết với nó như sau:</span><span class="sxs-lookup"><span data-stu-id="c54d2-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="c54d2-109">Ứng dụng OAuth sẽ có một thẻ có tên là "**Windowsazureactivedirecstafintegratedapp**"</span><span class="sxs-lookup"><span data-stu-id="c54d2-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="c54d2-110">Bộ sưu tập các ứng dụng SAML sẽ có thẻ có tên là "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="c54d2-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="c54d2-111">Ứng dụng không phải là bộ sưu tập SAML sẽ có thẻ có tên "**Windowsazureactivedirectorycustomsinglesignonapplication**"</span><span class="sxs-lookup"><span data-stu-id="c54d2-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="c54d2-112">Do đó, bạn có thể sử dụng các thẻ này và tìm hiểu xem loại ứng dụng đó là gì.</span><span class="sxs-lookup"><span data-stu-id="c54d2-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="c54d2-113">Thẻ "**Windowsazureactivedirectoryintegratedapp**" là chung cho tất cả các loại ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="c54d2-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="c54d2-114">Bạn có thể dùng đoạn trích sau đây để liệt kê tất cả các ứng dụng SAML (cả bộ sưu tập và không phải là bộ sưu tập):</span><span class="sxs-lookup"><span data-stu-id="c54d2-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="c54d2-115">Để biết thêm thông tin, hãy xem mục [xác định các ứng dụng SAML cho phép trong AZURE AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="c54d2-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="c54d2-116">**Chỉ tìm kiếm và danh sách các ứng dụng web**: dùng lệnh dưới đây để nhận tất cả các ứng dụng Azure AD với loại ứng dụng "Web App/API"</span><span class="sxs-lookup"><span data-stu-id="c54d2-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="c54d2-117">Get-AzureADApplication-tất cả: $true | Where-Object {$ _. PublicClient-NE $true} | Bình</span><span class="sxs-lookup"><span data-stu-id="c54d2-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="c54d2-118">**Tìm và danh sách các ứng dụng gốc một mình**: chạy lệnh sau đây để nhận tất cả các ứng dụng máy khách gốc (thiết bị di động/thiết bị di động).</span><span class="sxs-lookup"><span data-stu-id="c54d2-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="c54d2-119">Get-AzureADApplication-tất cả: $true | Where-Object {$ _. PublicClient-EQ $true} | Bình</span><span class="sxs-lookup"><span data-stu-id="c54d2-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="c54d2-120">**Xuất tất cả các chi tiết ứng dụng AZURE AD đã đăng ký thành CSV**: lệnh dưới đây xuất chuyển tất cả các ứng dụng Azure AD với chi tiết bắt buộc vào tệp CSV:</span><span class="sxs-lookup"><span data-stu-id="c54d2-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="c54d2-121">Get-AzureADApplication-tất cả: $true | Select-Object DisplayName, AppID, PublicClient, Availabletootherthuê, trang chủ, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="c54d2-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="c54d2-122">Export-Csv "C:\AzureADApps.csv"-thông tin mã hóa UTF8</span><span class="sxs-lookup"><span data-stu-id="c54d2-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="c54d2-123">**Cần xuất danh sách các ứng dụng Azure không sử dụng** – báo cáo kiểm nghiệm</span><span class="sxs-lookup"><span data-stu-id="c54d2-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="c54d2-124">Azure AD có thể hiển thị Nhật ký ứng dụng chỉ có tối đa 30 ngày cung cấp cho bạn giấy phép Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="c54d2-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="c54d2-125">Bạn có hai tùy chọn để giữ lại dữ liệu trong hơn 30 ngày.</span><span class="sxs-lookup"><span data-stu-id="c54d2-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="c54d2-126">Bạn có thể sử dụng [API báo cáo AZURE AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) để truy xuất các chương trình dữ liệu và lưu trữ nó trong một cơ sở dữ liệu.</span><span class="sxs-lookup"><span data-stu-id="c54d2-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="c54d2-127">Ngoài ra, bạn có thể tích hợp Nhật ký kiểm tra vào một hệ thống SIEM của bên thứ ba.</span><span class="sxs-lookup"><span data-stu-id="c54d2-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="c54d2-128">Bạn cũng có thể tải xuống danh sách ứng dụng cho tất cả các ứng dụng và các ứng dụng thuộc đối với đăng ký ứng dụng Azure Active Directory>>tải xuống>tất cả các ứng dụng/ứng dụng thuộc sở hữu.</span><span class="sxs-lookup"><span data-stu-id="c54d2-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="c54d2-129">Để lấy danh sách các ứng dụng thông qua MS graph, hãy xem [ứng dụng danh sách-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/application-list) và [loại tài nguyên ứng dụng-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="c54d2-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
