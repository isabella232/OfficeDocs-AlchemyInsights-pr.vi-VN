---
title: Thay đổi máy chủ tên
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714746"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="2afc6-102">Cập Nhật máy chủ tên miền của bạn để trỏ tới Microsoft</span><span class="sxs-lookup"><span data-stu-id="2afc6-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="2afc6-103">Lưu ý: những thay đổi máy chủ tên đôi khi có thể mất tới 48 giờ để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="2afc6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="2afc6-104">Để thiết lập tên miền của bạn trong Microsoft 365, máy chủ tên tại cơ quan đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="2afc6-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="2afc6-105">Tạo hoặc chỉnh sửa các bản ghi máy chủ tên tại cơ quan đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="2afc6-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="2afc6-106">Đi đến trang web của cơ quan đăng ký tên miền của bạn và tìm khu vực nơi bạn có thể sửa máy chủ tên.</span><span class="sxs-lookup"><span data-stu-id="2afc6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="2afc6-107">Tạo hoặc sửa hai bản ghi máy chủ tên để khớp với các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="2afc6-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="2afc6-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2afc6-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="2afc6-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2afc6-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="2afc6-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="2afc6-110">Save changes.</span></span>

<span data-ttu-id="2afc6-111">Bạn cũng có thể tìm thấy các hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên với bất kỳ cơ quan đăng ký tên miền nào](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="2afc6-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  