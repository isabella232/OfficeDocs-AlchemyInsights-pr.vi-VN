---
title: Thêm nhóm vào site SharePoint
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771230"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="9ec24-102">Các vấn đề khi tạo một site được kết nối nhóm trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="9ec24-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="9ec24-103">Một số vấn đề phổ biến gặp phải khi tạo hoặc tạo lại một trang kết nối nhóm.</span><span class="sxs-lookup"><span data-stu-id="9ec24-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="9ec24-104">Nếu bạn đã xóa một nhóm và site được kết nối và muốn tạo một site khác với cùng một URL, bạn sẽ cần loại bỏ vĩnh viễn site trước đó.</span><span class="sxs-lookup"><span data-stu-id="9ec24-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="9ec24-105">Tải xuống trình [bao quản lý SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="9ec24-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="9ec24-106">Để biết thêm thông tin về việc bắt đầu với PowerShell, hãy xem [bắt đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="9ec24-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="9ec24-107">Loại bỏ site khỏi các site đã xóa bằng lệnh ghép ngắn PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="9ec24-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="9ec24-108">PowerShell được yêu cầu để xóa vĩnh viễn các site nhóm.</span><span class="sxs-lookup"><span data-stu-id="9ec24-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="9ec24-109">Nếu bạn đang tạo một trang kết nối nhóm và nhận cảnh báo: **một nhóm khác với cùng một biệt danh đã tồn tại**, hãy kiểm tra các nhóm hiện có từ [Trung tâm quản trị Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="9ec24-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="9ec24-110">Để giải quyết sự cố này, hãy xóa nhóm hiện có nếu nó không còn cần thiết hoặc tạo site có một biệt danh khác được gán.</span><span class="sxs-lookup"><span data-stu-id="9ec24-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="9ec24-111">Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ec24-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="9ec24-112">Bạn có thể kết nối các site hiện có với một nhóm Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ec24-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="9ec24-113">Để biết thêm thông tin, hãy xem [kết nối nhóm Microsoft 365 bằng cách sử dụng giao diện người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="9ec24-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="9ec24-114">Để tạo site Microsoft 365 được kết nối, bạn sẽ cần tạo [site nhóm](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="9ec24-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
