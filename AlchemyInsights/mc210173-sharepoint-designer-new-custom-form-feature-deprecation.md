---
title: MC210173-SharePoint Designer mới tuỳ chỉnh mẫu tính năng kháng cáo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928549"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="5e18e-102">MC210173-SharePoint Designer mới tuỳ chỉnh mẫu tính năng kháng cáo</span><span class="sxs-lookup"><span data-stu-id="5e18e-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="5e18e-103">Chúng tôi đã xác định một vấn đề ảnh hưởng đến chức năng SharePoint Designer để [tạo biểu mẫu tuỳ chỉnh](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) trong SharePoint trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="5e18e-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="5e18e-104">Sau khi kiểm tra cẩn thận, chúng tôi đã xác định rằng không có sửa chữa được biết đến cho vấn đề này và có bầu để vô hiệu hoá tính năng tuỳ chỉnh tạo biểu mẫu có hiệu lực 3:00 AM UTC ngày thứ bảy, Tháng tư 25, 2020.</span><span class="sxs-lookup"><span data-stu-id="5e18e-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="5e18e-105">Thay đổi này không ảnh hưởng đến khả năng chỉnh sửa đã tạo mẫu hoặc các tính năng hiện có trong SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="5e18e-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="5e18e-106">Sau khi thay đổi này được thực hiện, người dùng có thể đã nhận được lỗi: "không thể lưu danh sách thay đổi máy chủ" khi tạo biểu mẫu mới.</span><span class="sxs-lookup"><span data-stu-id="5e18e-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="5e18e-107">Người dùng đã tận dụng SharePoint Designer để tạo tuỳ chỉnh mẫu thay vì có thể sử dụng [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) cho mục đích này.</span><span class="sxs-lookup"><span data-stu-id="5e18e-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="5e18e-108">PowerApps là một công cụ dễ dàng và mạnh mẽ cho phép người dùng hoạt động trong kinh nghiệm SharePoint Online hiện đại để tạo và chỉnh sửa biểu mẫu tuỳ chỉnh cho SharePoint danh sách và thư viện tài liệu ngay từ một cửa sổ trình duyệt.</span><span class="sxs-lookup"><span data-stu-id="5e18e-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="5e18e-109">PowerApps không yêu cầu kiến thức mã hóa truyền thống hoặc bất kỳ tải ứng dụng bổ sung như InfoPath.</span><span class="sxs-lookup"><span data-stu-id="5e18e-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="5e18e-110">**Lưu ý**: người dùng SharePoint Online Classic sẽ cần tạm thời chuyển sang trải nghiệm hiện đại để truy cập và sử dụng PowerApps; Tuy nhiên, tất cả các biểu mẫu tùy chỉnh được tạo trong PowerApps có thể truy cập bằng SharePoint Online Classic trải nghiệm người dùng.</span><span class="sxs-lookup"><span data-stu-id="5e18e-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
