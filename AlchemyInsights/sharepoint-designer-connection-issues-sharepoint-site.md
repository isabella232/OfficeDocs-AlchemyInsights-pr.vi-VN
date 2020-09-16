---
title: Các vấn đề về kết nối của SharePoint Designer
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
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727193"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="f8743-102">Các vấn đề về kết nối của SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="f8743-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="f8743-103">Nếu SharePoint Designer đang gặp vấn đề về kết nối với các site SharePoint, vui lòng thử các giải pháp thông thường sau đây.</span><span class="sxs-lookup"><span data-stu-id="f8743-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="f8743-104">Bước 1: xác minh rằng SharePoint Designer 2013 được Cập Nhật với [gói dịch vụ SharePoint Designer 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và bản [Cập Nhật 2 tháng tám 2016 cho SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="f8743-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="f8743-105">Bước 2: xóa các tệp bộ đệm ẩn cục bộ:</span><span class="sxs-lookup"><span data-stu-id="f8743-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="f8743-106">Đóng SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f8743-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="f8743-107">Trên máy tính cục bộ, hãy loại bỏ tất cả các tệp được tìm thấy trong mỗi thư mục sau đây.</span><span class="sxs-lookup"><span data-stu-id="f8743-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="f8743-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="f8743-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="f8743-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="f8743-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="f8743-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="f8743-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="f8743-111">Mở SharePoint Designer 2013 và nhập lại tài khoản để xem liệu nó có hoạt động hay không.</span><span class="sxs-lookup"><span data-stu-id="f8743-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="f8743-112">Bước 3: [bật xác thực hiện đại cho Office 2013 trên các thiết bị chạy Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f8743-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="f8743-113">Bước 4: người quản trị sẽ cần cho **phép các tập lệnh tùy chỉnh** trong thiết đặt Trung tâm quản trị SharePoint để cho phép kết nối SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="f8743-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="f8743-114">Xem mục [cho phép hoặc ngăn chặn các tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="f8743-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


