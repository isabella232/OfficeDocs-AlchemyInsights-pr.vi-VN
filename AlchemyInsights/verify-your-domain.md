---
title: Xác minh miền của bạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710465"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4b1c6-102">Xác minh miền của bạn</span><span class="sxs-lookup"><span data-stu-id="4b1c6-102">Verify your domain</span></span>

 <span data-ttu-id="4b1c6-103">**Bản ghi có thể đã không Cập Nhật trên Internet.**</span><span class="sxs-lookup"><span data-stu-id="4b1c6-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4b1c6-104">Nó thường chỉ mất vài phút để chúng tôi có thể xem các hồ sơ mới, nhưng đôi khi nó có thể mất miễn là một vài giờ.</span><span class="sxs-lookup"><span data-stu-id="4b1c6-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4b1c6-105">Nếu bạn đã chờ lâu rồi, hãy kiểm tra lại rằng bạn đã sao chép và dán giá trị chính xác vào bản ghi xác minh TXT tại máy chủ DNS của mình.</span><span class="sxs-lookup"><span data-stu-id="4b1c6-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4b1c6-106">Một vấn đề phổ biến không bao gồm "MS =" một phần của bản ghi.</span><span class="sxs-lookup"><span data-stu-id="4b1c6-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4b1c6-107">Chúng ta cũng cần điều đó!</span><span class="sxs-lookup"><span data-stu-id="4b1c6-107">We need that too!</span></span>

- <span data-ttu-id="4b1c6-108">Tại một số máy chủ DNS, bạn phải thực hiện thêm một bước để lưu tệp vùng (trong đó bản ghi DNS được lưu trữ) để nó sẽ cập nhật trên Internet.</span><span class="sxs-lookup"><span data-stu-id="4b1c6-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4b1c6-109">Đảm bảo rằng bạn đã lưu các thay đổi của mình để Microsoft có thể xem và xác minh bản ghi.</span><span class="sxs-lookup"><span data-stu-id="4b1c6-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
