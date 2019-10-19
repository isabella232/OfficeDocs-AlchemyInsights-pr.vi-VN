---
title: Thêm nhóm vào một trang web SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750542"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="00fd0-102">Vấn đề khi tạo hoặc nhóm các trang web được kết nối trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="00fd0-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="00fd0-103">Có một vài vấn đề phổ biến gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.</span><span class="sxs-lookup"><span data-stu-id="00fd0-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="00fd0-104">Nếu bạn đã xóa một nhóm và trang web được kết nối của nó và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần xóa vĩnh viễn trang web trước đó.</span><span class="sxs-lookup"><span data-stu-id="00fd0-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="00fd0-105">Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="00fd0-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="00fd0-106">Để biết thêm thông tin về việc bắt đầu với PowerShell, xem bắt [đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="00fd0-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="00fd0-107">Loại bỏ các trang web khỏi xóa các trang web bằng cách sử dụng lệnh ghép ngắn PowerShell [loại bỏ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="00fd0-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="00fd0-108">Nếu bạn đang tạo một nhóm kết nối trang web và nhận được cảnh báo một nhóm khác với cùng một bí danh đã tồn tại, kiểm tra các nhóm hiện có từ [Office 365 từ Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="00fd0-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="00fd0-109">Để khắc phục sự cố, xoá nhóm hiện có nếu nó không còn cần thiết hoặc tạo ra các trang web với một bí danh khác được chỉ định.</span><span class="sxs-lookup"><span data-stu-id="00fd0-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="00fd0-110">Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.</span><span class="sxs-lookup"><span data-stu-id="00fd0-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="00fd0-111">Bạn có thể kết nối các trang web hiện tại với một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="00fd0-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="00fd0-112">Để biết thêm thông tin, hãy xem [kết nối một nhóm Office 365 bằng cách sử dụng ineterface người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="00fd0-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="00fd0-113">Để tạo một trang web nhóm Office 365 được kết nối, bạn sẽ cần tạo một site nhóm.</span><span class="sxs-lookup"><span data-stu-id="00fd0-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="00fd0-114">Để biết thêm thông tin, xem [tạo trang web nhóm trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="00fd0-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

