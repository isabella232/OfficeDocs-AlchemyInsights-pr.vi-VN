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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496457"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="d694e-102">Chuyển đổi hộp thư người dùng vào hộp thư dùng chung</span><span class="sxs-lookup"><span data-stu-id="d694e-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="d694e-103">Bạn chỉ có thể chuyển đổi các hộp thư người dùng hộp thư dùng chung nếu người dùng có một giấy phép trao đổi.</span><span class="sxs-lookup"><span data-stu-id="d694e-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="d694e-104">Sau khi hộp thư được chuyển đổi, nó sẽ tiếp tục xuất hiện trong danh sách người dùng hoạt động bởi vì danh sách bao gồm hộp thư dùng chung.</span><span class="sxs-lookup"><span data-stu-id="d694e-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="d694e-105">Tuy nhiên, hộp thư đã được chuyển đổi sẽ cũng xuất hiện trong danh sách hộp thư dùng chung.</span><span class="sxs-lookup"><span data-stu-id="d694e-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d694e-106">Nếu bạn cố gắng để chuyển đổi các hộp thư trong giao diện điều khiển Admin đổi Ngoại tệ và chuyển đổi thất bại, xoá bộ nhớ cache của trình duyệt và cookie của bạn và thử lại.</span><span class="sxs-lookup"><span data-stu-id="d694e-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="d694e-107">Nếu nó vẫn không hoạt động, hãy thử chuyển đổi các hộp thư trong Exchange Management Shell bằng cách chạy lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="d694e-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d694e-108">Thông tin chuyển đổi hộp thư có sẵn trong [chuyển đổi hộp thư người dùng hộp thư dùng chung](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d694e-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
