---
title: OneDrive for Business web OneDrive chuyển hướng sang delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800011"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="61cac-102">Chuyển hướng đến delve sau khi bạn bấm vào OneDrive</span><span class="sxs-lookup"><span data-stu-id="61cac-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="61cac-103">Xem [hướng dẫn khắc phục sự cố](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)chi tiết của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="61cac-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="61cac-104">Để giải quyết vấn đề này, người quản trị phải cấp cho người dùng quyền tạo site trang của tôi.</span><span class="sxs-lookup"><span data-stu-id="61cac-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="61cac-105">Điều này là do trang OneDrive for Business được tạo trên site của tôi.</span><span class="sxs-lookup"><span data-stu-id="61cac-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="61cac-106">Để cấp quyền này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="61cac-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="61cac-107">Trong Trung tâm quản trị SharePoint, hãy bấm **hồ sơ người dùng**.</span><span class="sxs-lookup"><span data-stu-id="61cac-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="61cac-108">Trong mục **mọi người** , hãy bấm **quản lý quyền của người dùng**.</span><span class="sxs-lookup"><span data-stu-id="61cac-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="61cac-109">Thêm người dùng yêu cầu quyền để tạo trang site của tôi.</span><span class="sxs-lookup"><span data-stu-id="61cac-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="61cac-110">Theo mặc định, thiết đặt này được đặt là **tất cả mọi người, ngoại trừ người dùng bên ngoài**.</span><span class="sxs-lookup"><span data-stu-id="61cac-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="61cac-111">Sau khi đã thêm người dùng, người dùng hoặc nhóm, hãy đảm bảo rằng người dùng đã thêm, người dùng hoặc nhóm được chọn, cuộn đến phần **quyền** , rồi chọn hộp kiểm bên cạnh **tạo trang cá nhân (bắt buộc đối với lưu trữ cá nhân, nguồn cấp tin tức và nội dung được theo dõi)**.</span><span class="sxs-lookup"><span data-stu-id="61cac-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="61cac-112">Bấm **OK**, sau đó có người dùng duyệt đến trang OneDrive để tạo trang.</span><span class="sxs-lookup"><span data-stu-id="61cac-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
