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
Bạn chỉ có thể chuyển đổi các hộp thư người dùng hộp thư dùng chung nếu người dùng có một giấy phép trao đổi. Sau khi hộp thư được chuyển đổi, nó sẽ tiếp tục xuất hiện trong danh sách người dùng hoạt động bởi vì danh sách bao gồm hộp thư dùng chung. Tuy nhiên, hộp thư đã được chuyển đổi sẽ cũng xuất hiện trong danh sách hộp thư dùng chung. 
  
Nếu bạn cố gắng để chuyển đổi các hộp thư trong giao diện điều khiển Admin đổi Ngoại tệ và chuyển đổi thất bại, xoá bộ nhớ cache của trình duyệt và cookie của bạn và thử lại. Nếu nó vẫn không hoạt động, hãy thử chuyển đổi các hộp thư trong Exchange Management Shell bằng cách chạy lệnh sau:
  
```
Set-Mailbox -Type Shared
```

Thông tin chuyển đổi hộp thư có sẵn trong [chuyển đổi hộp thư người dùng hộp thư dùng chung](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
