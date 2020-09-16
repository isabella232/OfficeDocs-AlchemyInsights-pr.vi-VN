---
title: Cập Nhật máy chủ tên miền của bạn để trỏ tới Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734933"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="f9ebc-102">Cập Nhật máy chủ tên miền của bạn để trỏ tới Microsoft</span><span class="sxs-lookup"><span data-stu-id="f9ebc-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="f9ebc-103">Lưu ý: những thay đổi máy chủ tên đôi khi có thể mất tới 48 giờ để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="f9ebc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="f9ebc-104">Để thiết lập tên miền của bạn với Microsoft, máy chủ tên tại cơ quan đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="f9ebc-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="f9ebc-105">Tạo hoặc chỉnh sửa các bản ghi máy chủ tên tại cơ quan đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="f9ebc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="f9ebc-106">Đi đến trang web của cơ quan đăng ký tên miền của bạn và tìm khu vực nơi bạn có thể sửa máy chủ tên.</span><span class="sxs-lookup"><span data-stu-id="f9ebc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="f9ebc-107">Tạo hoặc sửa hai bản ghi máy chủ tên để khớp với các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="f9ebc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="f9ebc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f9ebc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="f9ebc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f9ebc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="f9ebc-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="f9ebc-110">Save changes.</span></span>

<span data-ttu-id="f9ebc-111">Bạn cũng có thể tìm thấy các hướng dẫn chi tiết trong bài viết này: thay đổi máy chủ tên [để thiết lập Microsoft 365 với bất kỳ cơ quan đăng ký tên miền nào](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="f9ebc-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  