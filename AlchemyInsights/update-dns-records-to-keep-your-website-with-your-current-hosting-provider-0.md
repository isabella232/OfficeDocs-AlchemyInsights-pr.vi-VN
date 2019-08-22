---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506429"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="40860-102">Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành</span><span class="sxs-lookup"><span data-stu-id="40860-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="40860-103">Trên trang [miền](https://portal.office.com/adminportal/home#/Domains) , trong danh sách các tên miền, chọn tên miền bạn đang sử dụng cho trang web của bạn.</span><span class="sxs-lookup"><span data-stu-id="40860-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="40860-104">Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="40860-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="40860-105">**DNS** loại nhập: **(địa chỉ)**</span><span class="sxs-lookup"><span data-stu-id="40860-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="40860-106">Đối với **tên máy chủ hoặc bí danh**, gõ như sau:**@**</span><span class="sxs-lookup"><span data-stu-id="40860-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="40860-107">Đối với **Địa chỉ IP**, gõ địa chỉ IP tĩnh cho trang web của bạn nơi mà nó hiện đang được tổ chức (ví dụ, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="40860-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="40860-108">Điều này phải có một địa chỉ IP *tĩnh* cho trang web, không phải là một địa chỉ IP *động* .</span><span class="sxs-lookup"><span data-stu-id="40860-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="40860-109">Kiểm tra với các trang web mà trang web của bạn được lưu trữ để đảm bảo rằng bạn có thể nhận được một địa chỉ IP tĩnh cho trang web công cộng của bạn.</span><span class="sxs-lookup"><span data-stu-id="40860-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="40860-110">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="40860-110">Select **Save**.</span></span>

<span data-ttu-id="40860-111">Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy trang web của bạn.</span><span class="sxs-lookup"><span data-stu-id="40860-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="40860-112">Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="40860-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="40860-113">**DNS** loại nhập: **CNAME (bí danh)**</span><span class="sxs-lookup"><span data-stu-id="40860-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="40860-114">Đối với **tên máy chủ hoặc bí danh**, gõ như sau: **www**</span><span class="sxs-lookup"><span data-stu-id="40860-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="40860-115">Cho **điểm đến địa chỉ**, hãy nhập tên miền đủ điều kiện (FQDN) cho trang web của bạn (ví dụ: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="40860-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="40860-116">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="40860-116">Select **Save**.</span></span>
