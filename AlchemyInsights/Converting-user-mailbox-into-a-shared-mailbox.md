---
title: Chuyển đổi hộp thư người dùng vào hộp thư dùng chung?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374345"
---
<span data-ttu-id="e44c8-102">Bạn chỉ có thể chuyển đổi các hộp thư người dùng hộp thư dùng chung nếu người dùng có một giấy phép trao đổi.</span><span class="sxs-lookup"><span data-stu-id="e44c8-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="e44c8-103">Sau khi hộp thư được chuyển đổi, nó sẽ tiếp tục xuất hiện trong danh sách người dùng hoạt động bởi vì danh sách bao gồm hộp thư dùng chung.</span><span class="sxs-lookup"><span data-stu-id="e44c8-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="e44c8-104">Tuy nhiên, hộp thư đã được chuyển đổi sẽ cũng xuất hiện trong danh sách hộp thư dùng chung.</span><span class="sxs-lookup"><span data-stu-id="e44c8-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="e44c8-105">Nếu bạn cố gắng để chuyển đổi các hộp thư trong giao diện điều khiển Admin đổi Ngoại tệ và chuyển đổi thất bại, xoá bộ nhớ cache của trình duyệt và cookie của bạn và thử lại.</span><span class="sxs-lookup"><span data-stu-id="e44c8-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="e44c8-106">Nếu nó vẫn không hoạt động, hãy thử chuyển đổi các hộp thư trong Exchange Management Shell bằng cách chạy lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="e44c8-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="e44c8-107">Thông tin chuyển đổi hộp thư có sẵn trong [chuyển đổi hộp thư người dùng hộp thư dùng chung](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="e44c8-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
