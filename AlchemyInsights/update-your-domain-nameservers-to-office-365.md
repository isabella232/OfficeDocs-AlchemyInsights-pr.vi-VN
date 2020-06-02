---
title: Cập Nhật máy máy chủ tên miền của bạn để trỏ tới Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510306"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="fef61-102">Cập Nhật máy máy chủ tên miền của bạn để trỏ tới Microsoft</span><span class="sxs-lookup"><span data-stu-id="fef61-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="fef61-103">Lưu ý: thay đổi nameserver đôi khi có thể mất đến 48 giờ để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="fef61-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="fef61-104">Để thiết lập miền của bạn với Microsoft, máy chủ tên tại công ty đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="fef61-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="fef61-105">Tạo hoặc chỉnh sửa hồ sơ nameserver của bạn tại công ty đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="fef61-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="fef61-106">Truy cập trang web của công ty đăng ký tên miền của bạn và tìm khu vực nơi bạn có thể chỉnh sửa tên máy Nameservers.</span><span class="sxs-lookup"><span data-stu-id="fef61-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="fef61-107">Tạo hoặc chỉnh sửa hai nameserver bản ghi để phù hợp với các giá trị:</span><span class="sxs-lookup"><span data-stu-id="fef61-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="fef61-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fef61-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="fef61-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fef61-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="fef61-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="fef61-110">Save changes.</span></span>

<span data-ttu-id="fef61-111">Bạn cũng có thể tìm thấy hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên để thiết lập Microsoft 365 với bất kỳ công ty đăng ký tên miền](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="fef61-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  