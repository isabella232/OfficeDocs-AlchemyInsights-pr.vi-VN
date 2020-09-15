---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699541"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="325d3-102">Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại</span><span class="sxs-lookup"><span data-stu-id="325d3-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="325d3-103">Trong Trung tâm quản trị Microsoft 365, hãy đi **Setup**đến  >  trang[tên miền](https://portal.office.com/adminportal/home#/Domains) thiết lập và trong danh sách tên miền, chọn tên miền mà bạn đang sử dụng cho website của bạn.</span><span class="sxs-lookup"><span data-stu-id="325d3-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="325d3-104">Chọn **+ bản ghi tùy chỉnh mới** và nhập nội dung sau đây:</span><span class="sxs-lookup"><span data-stu-id="325d3-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="325d3-105">Đối với **loại DNS** , hãy nhập: **A (địa chỉ)**</span><span class="sxs-lookup"><span data-stu-id="325d3-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="325d3-106">Đối với **tên máy chủ hoặc biệt danh**, hãy nhập các tùy chọn sau: **@**</span><span class="sxs-lookup"><span data-stu-id="325d3-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="325d3-107">Đối với **địa chỉ IP**, hãy nhập địa chỉ IP tĩnh cho trang web của bạn tại vị trí hiện tại được lưu trữ (ví dụ,: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="325d3-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="325d3-108">Đây phải là một địa chỉ IP  *tĩnh*  cho trang web, chứ không phải địa chỉ IP  *động*  .</span><span class="sxs-lookup"><span data-stu-id="325d3-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="325d3-109">Kiểm tra với site nơi lưu trữ website của bạn để đảm bảo rằng bạn có thể nhận được địa chỉ IP tĩnh cho trang web công cộng của bạn.</span><span class="sxs-lookup"><span data-stu-id="325d3-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="325d3-110">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="325d3-110">Select **Save**.</span></span>

<span data-ttu-id="325d3-111">Ngoài ra, bạn có thể tạo một bản ghi CNAME để giúp khách hàng tìm thấy website của bạn.</span><span class="sxs-lookup"><span data-stu-id="325d3-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="325d3-112">Chọn **+ bản ghi tùy chỉnh mới** và nhập nội dung sau đây:</span><span class="sxs-lookup"><span data-stu-id="325d3-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="325d3-113">Đối với **loại DNS** , hãy nhập: **CNAME (biệt danh)**</span><span class="sxs-lookup"><span data-stu-id="325d3-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="325d3-114">Đối với **tên máy chủ hoặc biệt danh**, hãy gõ như sau: **www**</span><span class="sxs-lookup"><span data-stu-id="325d3-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="325d3-115">Đối với **trỏ tới địa chỉ**, hãy nhập tên miền đủ điều kiện (FQDN) cho website của bạn (ví dụ, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="325d3-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="325d3-116">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="325d3-116">Select **Save**.</span></span>
