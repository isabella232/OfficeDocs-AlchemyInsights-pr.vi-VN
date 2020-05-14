---
title: Thêm nhóm vào một trang web SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064415"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="9cdfb-102">Vấn đề khi tạo một nhóm kết nối trang web trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="9cdfb-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="9cdfb-103">Một số vấn đề phổ biến gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="9cdfb-104">Nếu bạn đã xóa một nhóm và trang web được kết nối của nó và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần xóa vĩnh viễn trang web trước đó.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="9cdfb-105">Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="9cdfb-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="9cdfb-106">Để biết thêm thông tin về việc bắt đầu với PowerShell, xem bắt [đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="9cdfb-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="9cdfb-107">Loại bỏ các trang web khỏi xóa các trang web bằng cách sử dụng lệnh ghép ngắn PowerShell [loại bỏ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="9cdfb-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="9cdfb-108">PowerShell là bắt buộc để xóa vĩnh viễn các trang web nhóm.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="9cdfb-109">Nếu bạn đang tạo trang web được kết nối nhóm và nhận cảnh báo: **một nhóm khác có cùng bí danh đã tồn tại**, hãy kiểm tra các nhóm hiện có từ [Trung tâm quản trị Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="9cdfb-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="9cdfb-110">Để khắc phục sự cố, xoá nhóm hiện có nếu nó không còn cần thiết hoặc tạo ra các trang web với một bí danh khác được chỉ định.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="9cdfb-111">Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="9cdfb-112">Bạn có thể kết nối các trang web hiện có với một nhóm Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9cdfb-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="9cdfb-113">Để biết thêm thông tin, hãy xem [kết nối nhóm Microsoft 365 bằng cách sử dụng giao diện người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="9cdfb-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="9cdfb-114">Để tạo một trang web được kết nối với nhóm Microsoft 365, bạn cần tạo một [site nhóm](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="9cdfb-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
