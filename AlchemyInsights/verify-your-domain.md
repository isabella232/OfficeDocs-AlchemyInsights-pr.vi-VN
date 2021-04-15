---
title: Xác nhận tên miền của bạn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771013"
---
# <a name="verify-your-domain"></a><span data-ttu-id="5b9a2-102">Xác nhận tên miền của bạn</span><span class="sxs-lookup"><span data-stu-id="5b9a2-102">Verify your domain</span></span>

 <span data-ttu-id="5b9a2-103">**Bản ghi có thể không được Cập Nhật trên Internet.**</span><span class="sxs-lookup"><span data-stu-id="5b9a2-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="5b9a2-104">Thông thường chỉ mất vài phút để chúng tôi có thể nhìn thấy bản ghi mới nhưng đôi khi có thể mất nhiều giờ.</span><span class="sxs-lookup"><span data-stu-id="5b9a2-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="5b9a2-105">Nếu bạn đã đợi lâu đã có, hãy kiểm tra lại rằng bạn đã sao chép và dán giá trị chính xác vào bản ghi xác minh TXT tại máy chủ DNS của bạn.</span><span class="sxs-lookup"><span data-stu-id="5b9a2-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="5b9a2-106">Một vấn đề phổ biến không bao gồm "MS =" là một phần của bản ghi.</span><span class="sxs-lookup"><span data-stu-id="5b9a2-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="5b9a2-107">Chúng tôi cần quá!</span><span class="sxs-lookup"><span data-stu-id="5b9a2-107">We need that too!</span></span>

- <span data-ttu-id="5b9a2-108">Tại một số máy chủ DNS, bạn phải thực hiện một bước bổ sung để lưu tệp vùng (nơi lưu trữ bản ghi DNS) để nó sẽ cập nhật qua Internet.</span><span class="sxs-lookup"><span data-stu-id="5b9a2-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="5b9a2-109">Hãy đảm bảo rằng bạn đã lưu các thay đổi của mình để Microsoft có thể xem và xác nhận bản ghi.</span><span class="sxs-lookup"><span data-stu-id="5b9a2-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
