---
title: Thêm một nhóm cho một trang web SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507869"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="0a396-102">Vấn đề khi tạo hoặc nhóm kết nối các trang web trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0a396-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="0a396-103">Không có một vài vấn đề thường gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.</span><span class="sxs-lookup"><span data-stu-id="0a396-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="0a396-104">Nếu bạn đã xoá một nhóm và trang web được kết nối và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần để vĩnh viễn loại bỏ trang web trước đó.</span><span class="sxs-lookup"><span data-stu-id="0a396-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="0a396-105">Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="0a396-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="0a396-106">Để biết thêm chi tiết trên bắt đầu bằng powershell, hãy xem [bắt đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="0a396-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="0a396-107">Loại bỏ các trang web từ xóa các trang web bằng cách sử dụng lệnh ghép ngắn powershell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="0a396-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="0a396-108">Nếu bạn đang tạo ra một nhóm kết nối trang web và nhận được một cảnh báo nhóm khác với bí danh cùng đã tồn tại, hãy kiểm tra các nhóm hiện có từ [Office 365 từ Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="0a396-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="0a396-109">Để giải quyết vấn đề, xóa nhóm hiện tại nếu nó không còn cần thiết hoặc tạo ra các trang web với một biệt danh khác nhau được chỉ định.</span><span class="sxs-lookup"><span data-stu-id="0a396-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="0a396-110">Có những cách khác nhau để tạo ra và sử dụng các nhóm hiện đại với SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0a396-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="0a396-111">Bạn có thể kết nối trang web hiện có với một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="0a396-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="0a396-112">Để biết thêm chi tiết, hãy xem [kết nối một nhóm Office 365 sử dụng SharePoint người dùng ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="0a396-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="0a396-113">Để tạo một trang web được kết nối nhóm Office 365, bạn cần tạo một trang web đội ngũ.</span><span class="sxs-lookup"><span data-stu-id="0a396-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="0a396-114">Để biết thêm chi tiết, hãy xem [tạo một nhóm trang web trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="0a396-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

