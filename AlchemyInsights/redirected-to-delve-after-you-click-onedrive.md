---
title: OneDrive for Business web OneDrive chuyển hướng sang delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776402"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="a522b-102">Chuyển hướng đến delve sau khi bạn bấm vào OneDrive</span><span class="sxs-lookup"><span data-stu-id="a522b-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="a522b-103">Xem [hướng dẫn khắc phục sự cố](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)chi tiết của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="a522b-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="a522b-104">Để giải quyết vấn đề này, người quản trị phải cấp cho người dùng quyền tạo site trang của tôi.</span><span class="sxs-lookup"><span data-stu-id="a522b-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="a522b-105">Điều này là do trang OneDrive for Business được tạo trên site của tôi.</span><span class="sxs-lookup"><span data-stu-id="a522b-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="a522b-106">Để cấp quyền này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="a522b-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="a522b-107">Trong Trung tâm quản trị SharePoint, hãy bấm **hồ sơ người dùng**.</span><span class="sxs-lookup"><span data-stu-id="a522b-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="a522b-108">Trong mục **mọi người** , hãy bấm **quản lý quyền của người dùng**.</span><span class="sxs-lookup"><span data-stu-id="a522b-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="a522b-109">Thêm người dùng yêu cầu quyền để tạo trang site của tôi.</span><span class="sxs-lookup"><span data-stu-id="a522b-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="a522b-110">Theo mặc định, thiết đặt này được đặt là **tất cả mọi người, ngoại trừ người dùng bên ngoài**.</span><span class="sxs-lookup"><span data-stu-id="a522b-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="a522b-111">Sau khi đã thêm người dùng, người dùng hoặc nhóm, hãy đảm bảo rằng người dùng đã thêm, người dùng hoặc nhóm được chọn, cuộn đến phần **quyền** , rồi chọn hộp kiểm bên cạnh **tạo trang cá nhân (bắt buộc đối với lưu trữ cá nhân, nguồn cấp tin tức và nội dung được theo dõi)**.</span><span class="sxs-lookup"><span data-stu-id="a522b-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="a522b-112">Bấm **OK**, sau đó có người dùng duyệt đến trang OneDrive để tạo trang.</span><span class="sxs-lookup"><span data-stu-id="a522b-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
