---
title: Vấn đề kết nối SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840573"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="74ae7-102">Vấn đề kết nối SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="74ae7-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="74ae7-103">Nếu SharePoint Designer gặp phải vấn đề kết nối với các trang web SharePoint, vui lòng thử các giải pháp phổ biến sau.</span><span class="sxs-lookup"><span data-stu-id="74ae7-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="74ae7-104">Bước 1: Xác minh rằng SharePoint Designer 2013 được Cập Nhật với [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và [2 tháng tám năm 2016 Cập Nhật cho SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="74ae7-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="74ae7-105">Bước 2: Xóa các tập tin bộ đệm ẩn cục bộ:</span><span class="sxs-lookup"><span data-stu-id="74ae7-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="74ae7-106">Đóng SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="74ae7-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="74ae7-107">Trên máy tính, loại bỏ tất cả các file trong mỗi thư mục sau đây được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="74ae7-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="74ae7-108">%AppData%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="74ae7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="74ae7-109">%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="74ae7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="74ae7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="74ae7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="74ae7-111">Mở SharePoint Designer 2013 và nhập vào tài khoản một lần nữa để xem nếu nó hoạt động.</span><span class="sxs-lookup"><span data-stu-id="74ae7-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="74ae7-112">Bước 3: Cho [phép xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="74ae7-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="74ae7-113">Bước 4: Quản trị viên sẽ cần phải **Cho phép tuỳ chỉnh Script** trong các thiết lập Trung tâm quản trị SharePoint cho phép kết nối SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="74ae7-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="74ae7-114">Xem [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) cho biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="74ae7-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


