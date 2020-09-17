---
title: Exchange PowerShell và tính năng xác thực cơ bản
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782997"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell và tính năng xác thực cơ bản

Để biết thông tin mới nhất về cách kết nối với Exchange Online PowerShell mà không cần phải sử dụng xác thực cơ bản, [vui lòng đến đây](https://aka.ms/exops-docs). Mô-đun PowerShell v2 sẽ không dùng xác thực cơ bản.

Xin lưu ý rằng xác thực cơ bản vẫn cần được kích hoạt trên máy khách của bạn.
Mô-đun PowerShell mới v2 dùng Auth hiện đại để thiết lập kết nối cho việc cho phép tất cả các lệnh ghép ngắn v2 dựa trên phần còn lại. Ngoài các lệnh ghép ngắn v2, nó cũng cho phép bạn truy nhập các lệnh ghép ngắn PowerShell từ xa cũ hơn (RPS), yêu cầu phải được thiết lập phiên làm việc PowerShell từ xa. Thiết lập một phiên RPS trên Windows Machine yêu cầu WinRM BasicAuth được kích hoạt trên máy khách ngay cả khi mô-đun sử dụng cơ chế xác thực hiện đại để xác thực dịch vụ. Đường ống WinRM cơ bản được sử dụng để vận chuyển các thẻ xác thực hiện đại. Nếu WinRM cơ bản được tắt trên máy khách, các lệnh ghép ngắn v2 mới sẽ tiếp tục làm việc (nhưng các lệnh ghép ngắn RPS cũ hơn sẽ không).
