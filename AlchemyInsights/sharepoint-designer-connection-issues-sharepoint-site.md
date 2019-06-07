---
title: Cấp phép SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760714"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="37285-102">Vấn đề kết nối SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="37285-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="37285-103">Nếu SharePoint Designer gặp phải vấn đề kết nối với các trang web SharePoint, xin vui lòng thử các giải pháp phổ biến sau.</span><span class="sxs-lookup"><span data-stu-id="37285-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="37285-104">Bước 1: Xác minh SharePoint Designer được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="37285-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="37285-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="37285-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="37285-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="37285-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="37285-107">Cập Nhật cho SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="37285-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="37285-108">Bước 2: Xóa các tập tin bộ đệm ẩn cục bộ</span><span class="sxs-lookup"><span data-stu-id="37285-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="37285-109">Đóng SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="37285-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="37285-110">Trên máy tính địa phương, trình duyệt các thư mục sau đây để loại bỏ các tập tin lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="37285-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="37285-111">Click vào Start, Run và xóa tất cả các tập tin được tìm thấy dưới mỗi của các bên dưới vị trí.</span><span class="sxs-lookup"><span data-stu-id="37285-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="37285-112">Máy chủ %AppData%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="37285-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="37285-113">Mở SharePoint Designer 2013 và nhập vào tài khoản một lần nữa để xem nếu nó hoạt động.</span><span class="sxs-lookup"><span data-stu-id="37285-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="37285-114">Bước 3: Cho [phép xác thực hiện đại cho Office 2013 trên cửa sổ thiết bị](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="37285-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="37285-115">Bước 4: Quản trị viên sẽ cần phải cho phép tuỳ chỉnh Script cho phép kết nối SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="37285-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="37285-116">Bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="37285-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


