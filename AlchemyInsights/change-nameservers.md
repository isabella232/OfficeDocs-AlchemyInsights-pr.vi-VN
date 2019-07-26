---
title: Thay đổi máy chủ tên
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902951"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="339cf-102">Cập Nhật máy chủ tên miền của bạn vào Office 365</span><span class="sxs-lookup"><span data-stu-id="339cf-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="339cf-103">Lưu ý: Thay đổi Nameserver đôi khi có thể mất đến 48 giờ để truyền bá.</span><span class="sxs-lookup"><span data-stu-id="339cf-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="339cf-104">Để thiết lập tên miền của bạn vào Office 365, các máy chủ tên lúc đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="339cf-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="339cf-105">Tạo hoặc chỉnh sửa hồ sơ nameserver của bạn tại công ty đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="339cf-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="339cf-106">Đi đến trang web của nhà cung cấp miền của bạn và tìm thấy các khu vực nơi bạn có thể chỉnh sửa các máy chủ tên.</span><span class="sxs-lookup"><span data-stu-id="339cf-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="339cf-107">Tạo hoặc chỉnh sửa hai máy chủ tên hồ sơ để phù hợp với các giá trị:</span><span class="sxs-lookup"><span data-stu-id="339cf-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="339cf-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="339cf-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="339cf-109">ns2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="339cf-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="339cf-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="339cf-110">Save changes.</span></span>

<span data-ttu-id="339cf-111">Bạn cũng có thể tìm thấy hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên để thiết lập Office 365 với bất kỳ đăng ký tên miền](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="339cf-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  