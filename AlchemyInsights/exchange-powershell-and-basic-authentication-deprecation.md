---
title: Exchange Việc bỏ dùng PowerShell và xác thực cơ bản
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069266"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange Việc bỏ dùng PowerShell và xác thực cơ bản

Để biết thông tin mới nhất về cách kết nối Exchange Online PowerShell mà không sử dụng Xác thực Cơ bản, [vui lòng truy cập vào đây.](https://aka.ms/exops-docs) Mô-đun PowerShell V2 không sử dụng xác thực cơ bản.

Vui lòng lưu ý rằng bạn vẫn cần bật Xác thực Cơ bản trên máy khách.
Mô-đun PowerShell V2 mới sử dụng Xác thực Hiện đại để thiết lập kết nối cho phép tất cả lệnh ghép ngắn V2 dựa trên REST. Ngoài lệnh ghép ngắn V2, lệnh ghép ngắn này cũng cho phép bạn truy nhập lệnh ghép ngắn Remote PowerShell (RPS) cũ hơn, lệnh ghép ngắn này đòi hỏi phải thiết lập phiên Làm việc PowerShell Từ xa. Để thiết lập phiên RPS trên máy Windows cần bật WinRM BasicAuth trên máy khách ngay cả khi mô-đun sử dụng cơ chế Xác thực Hiện đại để xác thực dịch vụ. Ống dẫn Xác thực Cơ bản WinRM được dùng để chuyển các mã thông báo Xác thực Hiện đại. Nếu WinRM Basic Auth bị vô hiệu hóa trên máy khách, các lệnh ghép ngắn V2 mới sẽ tiếp tục hoạt động (nhưng các lệnh ghép ngắn RPS cũ hơn sẽ không hoạt động).
