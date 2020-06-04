---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665782"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="04550-102">Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại</span><span class="sxs-lookup"><span data-stu-id="04550-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="04550-103">Trong Trung tâm quản trị Microsoft 365, hãy đi tới trang **thiết lập**  >  [miền](https://portal.office.com/adminportal/home#/Domains) và trong danh sách tên miền, chọn miền bạn đang sử dụng cho trang web của mình.</span><span class="sxs-lookup"><span data-stu-id="04550-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="04550-104">Chọn **+ bản ghi tùy chỉnh mới** và nhập các mục sau:</span><span class="sxs-lookup"><span data-stu-id="04550-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="04550-105">Đối với **loại DNS** nhập: **A (địa chỉ)**</span><span class="sxs-lookup"><span data-stu-id="04550-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="04550-106">**Tên máy chủ hoặc bí danh**, gõ như sau:**@**</span><span class="sxs-lookup"><span data-stu-id="04550-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="04550-107">Đối với **địa chỉ IP**, nhập địa chỉ IP tĩnh cho trang web của bạn nơi hiện đang lưu trữ (ví dụ: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="04550-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="04550-108">Điều này phải là một địa chỉ IP *tĩnh* cho các trang web, không một địa chỉ IP *động* .</span><span class="sxs-lookup"><span data-stu-id="04550-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="04550-109">Kiểm tra với trang web nơi trang web của bạn được lưu trữ để đảm bảo bạn có thể nhận được một địa chỉ IP tĩnh cho trang web công cộng của bạn.</span><span class="sxs-lookup"><span data-stu-id="04550-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="04550-110">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="04550-110">Select **Save**.</span></span>

<span data-ttu-id="04550-111">Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy trang web của bạn.</span><span class="sxs-lookup"><span data-stu-id="04550-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="04550-112">Chọn **+ bản ghi tùy chỉnh mới** và nhập các mục sau:</span><span class="sxs-lookup"><span data-stu-id="04550-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="04550-113">Đối với **loại DNS** nhập: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="04550-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="04550-114">**Tên máy chủ hoặc bí danh**, gõ như sau: **www**</span><span class="sxs-lookup"><span data-stu-id="04550-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="04550-115">Đối **với điểm đến địa chỉ**, nhập tên miền đủ điều kiện (FQDN) cho trang web của bạn (ví dụ: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="04550-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="04550-116">Chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="04550-116">Select **Save**.</span></span>
