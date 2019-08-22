---
title: Cập Nhật máy chủ tên miền của bạn vào Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506069"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="bdbe4-102">Cập Nhật máy chủ tên miền của bạn vào Office 365</span><span class="sxs-lookup"><span data-stu-id="bdbe4-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="bdbe4-103">Lưu ý: Thay đổi Nameserver đôi khi có thể mất đến 48 giờ để truyền bá.</span><span class="sxs-lookup"><span data-stu-id="bdbe4-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="bdbe4-104">Để thiết lập tên miền của bạn vào Office 365, các máy chủ tên lúc đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="bdbe4-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="bdbe4-105">Tạo hoặc chỉnh sửa hồ sơ nameserver của bạn tại công ty đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="bdbe4-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="bdbe4-106">Đi đến trang web của nhà cung cấp miền của bạn và tìm thấy các khu vực nơi bạn có thể chỉnh sửa các máy chủ tên.</span><span class="sxs-lookup"><span data-stu-id="bdbe4-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="bdbe4-107">Tạo hoặc chỉnh sửa hai máy chủ tên hồ sơ để phù hợp với các giá trị:</span><span class="sxs-lookup"><span data-stu-id="bdbe4-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="bdbe4-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bdbe4-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="bdbe4-109">ns2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bdbe4-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="bdbe4-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="bdbe4-110">Save changes.</span></span>

<span data-ttu-id="bdbe4-111">Bạn cũng có thể tìm thấy hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên để thiết lập Office 365 với bất kỳ đăng ký tên miền](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="bdbe4-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  