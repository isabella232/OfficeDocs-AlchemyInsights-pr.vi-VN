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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Chuyển đổi hộp thư người dùng vào hộp thư dùng chung

Bạn chỉ có thể chuyển đổi các hộp thư người dùng hộp thư dùng chung nếu người dùng có một giấy phép trao đổi. Sau khi hộp thư được chuyển đổi, nó sẽ tiếp tục xuất hiện trong danh sách người dùng hoạt động bởi vì danh sách bao gồm hộp thư dùng chung. Tuy nhiên, hộp thư đã được chuyển đổi sẽ cũng xuất hiện trong danh sách hộp thư dùng chung. 
  
Nếu bạn cố gắng để chuyển đổi các hộp thư trong giao diện điều khiển Admin đổi Ngoại tệ và chuyển đổi thất bại, xoá bộ nhớ cache của trình duyệt và cookie của bạn và thử lại. Nếu nó vẫn không hoạt động, hãy thử chuyển đổi các hộp thư trong Exchange Management Shell bằng cách chạy lệnh sau:
  
```
Set-Mailbox -Type Shared
```

Thông tin chuyển đổi hộp thư có sẵn trong [chuyển đổi hộp thư người dùng hộp thư dùng chung](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
