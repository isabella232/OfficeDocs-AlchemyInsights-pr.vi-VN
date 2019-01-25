---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496988"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="58f1f-102">Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành</span><span class="sxs-lookup"><span data-stu-id="58f1f-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="58f1f-103">Trên trang [miền](https://portal.office.com/adminportal/home#/Domains) , trong danh sách các tên miền, chọn tên miền bạn đang sử dụng cho trang web của bạn, và sau đó chọn **cài đặt DNS** trong cửa sổ quản lý.</span><span class="sxs-lookup"><span data-stu-id="58f1f-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="58f1f-104">Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="58f1f-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="58f1f-105">**DNS** loại nhập: **(địa chỉ)**</span><span class="sxs-lookup"><span data-stu-id="58f1f-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="58f1f-106">Đối với **tên máy chủ hoặc bí danh**, gõ như sau:**@**</span><span class="sxs-lookup"><span data-stu-id="58f1f-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="58f1f-107">Đối với **Địa chỉ IP**, gõ địa chỉ IP tĩnh cho trang web của bạn nơi mà nó hiện đang được tổ chức (ví dụ, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="58f1f-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="58f1f-p101">Điều này phải có một địa chỉ IP *tĩnh* cho trang web, không phải là một địa chỉ IP *động* . Kiểm tra với các trang web mà trang web của bạn được lưu trữ để đảm bảo rằng bạn có thể nhận được một địa chỉ IP tĩnh cho trang web công cộng của bạn.</span><span class="sxs-lookup"><span data-stu-id="58f1f-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="58f1f-110">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="58f1f-110">Select **Save**.</span></span> 
    
<span data-ttu-id="58f1f-111">Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy trang web của bạn.</span><span class="sxs-lookup"><span data-stu-id="58f1f-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="58f1f-112">Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="58f1f-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="58f1f-113">**DNS** loại nhập: **CNAME (bí danh)**</span><span class="sxs-lookup"><span data-stu-id="58f1f-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="58f1f-114">Đối với **tên máy chủ hoặc bí danh**, gõ như sau: **www**</span><span class="sxs-lookup"><span data-stu-id="58f1f-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="58f1f-115">Cho **điểm đến địa chỉ**, hãy nhập tên miền đủ điều kiện (FQDN) cho trang web của bạn (ví dụ: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="58f1f-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="58f1f-116">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="58f1f-116">Select **Save**.</span></span> 
    

