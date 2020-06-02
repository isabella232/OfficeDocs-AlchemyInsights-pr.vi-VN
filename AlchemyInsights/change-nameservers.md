---
title: Thay đổi NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508110"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="20351-102">Cập Nhật máy máy chủ tên miền của bạn để trỏ tới Microsoft</span><span class="sxs-lookup"><span data-stu-id="20351-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="20351-103">Lưu ý: thay đổi nameserver đôi khi có thể mất đến 48 giờ để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="20351-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="20351-104">Để thiết lập miền của bạn trong Microsoft 365, tên đăng ký của bạn cần phải được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="20351-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="20351-105">Tạo hoặc chỉnh sửa hồ sơ nameserver của bạn tại công ty đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="20351-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="20351-106">Truy cập trang web của công ty đăng ký tên miền của bạn và tìm khu vực nơi bạn có thể chỉnh sửa tên máy Nameservers.</span><span class="sxs-lookup"><span data-stu-id="20351-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="20351-107">Tạo hoặc chỉnh sửa hai nameserver bản ghi để phù hợp với các giá trị:</span><span class="sxs-lookup"><span data-stu-id="20351-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="20351-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="20351-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="20351-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="20351-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="20351-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="20351-110">Save changes.</span></span>

<span data-ttu-id="20351-111">Bạn cũng có thể tìm thấy hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên với bất kỳ đăng ký tên miền](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="20351-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  