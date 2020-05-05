---
title: Exchange PowerShell và sự phản kháng xác thực cơ bản
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015711"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell và sự phản kháng xác thực cơ bản

Để biết thông tin mới nhất về cách kết nối với Exchange Online PowerShell mà không cần sử dụng xác thực cơ bản, [vui lòng truy cập ở đây](https://aka.ms/psbasicauth).

Xin lưu ý rằng xác thực cơ bản vẫn cần phải được kích hoạt trên máy khách của bạn.
Mô-đun PowerShell v2 mới sử dụng hiện đại Auth để thiết lập kết nối cho phép tất cả các lệnh ghép ngắn v2 dựa trên phần còn lại. Ngoài các lệnh ghép ngắn v2, nó cũng cho phép bạn truy cập các lệnh ghép ngắn PowerShell từ xa (RPS) cũ hơn yêu cầu phiên PowerShell từ xa được thiết lập. Thiết lập một phiên RPS trên máy Windows yêu cầu WinRM BasicAuth được kích hoạt trên máy khách mặc dù mô-đun sử dụng cơ chế hiện đại Auth để xác thực dịch vụ. Đường ống WinRM cơ bản Auth được sử dụng để vận chuyển các token hiện đại Auth. Nếu WinRM cơ bản Auth bị vô hiệu hoá trên máy khách, lệnh ghép ngắn v2 mới sẽ tiếp tục hoạt động (nhưng cũ RPS lệnh ghép ngắn sẽ không).
