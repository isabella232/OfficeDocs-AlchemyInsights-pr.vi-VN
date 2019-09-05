---
title: Thay đổi NameServers
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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736671"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="52c18-102">Cập Nhật máy máy chủ tên miền của bạn để Office 365</span><span class="sxs-lookup"><span data-stu-id="52c18-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="52c18-103">Lưu ý: thay đổi nameserver đôi khi có thể mất đến 48 giờ để tuyên truyền.</span><span class="sxs-lookup"><span data-stu-id="52c18-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="52c18-104">Để thiết lập miền của bạn trong Office 365, máy tên đăng ký của bạn cần được Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="52c18-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="52c18-105">Tạo hoặc chỉnh sửa hồ sơ nameserver của bạn tại công ty đăng ký tên miền của bạn.</span><span class="sxs-lookup"><span data-stu-id="52c18-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="52c18-106">Truy cập trang web của công ty đăng ký tên miền của bạn và tìm khu vực nơi bạn có thể chỉnh sửa tên máy Nameservers.</span><span class="sxs-lookup"><span data-stu-id="52c18-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="52c18-107">Tạo hoặc chỉnh sửa hai nameserver bản ghi để phù hợp với các giá trị:</span><span class="sxs-lookup"><span data-stu-id="52c18-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="52c18-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="52c18-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="52c18-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="52c18-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="52c18-110">Lưu thay đổi.</span><span class="sxs-lookup"><span data-stu-id="52c18-110">Save changes.</span></span>

<span data-ttu-id="52c18-111">Bạn cũng có thể tìm thấy hướng dẫn chi tiết trong bài viết này: [thay đổi máy chủ tên để thiết lập Office 365 với bất kỳ công ty đăng ký tên miền](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="52c18-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  