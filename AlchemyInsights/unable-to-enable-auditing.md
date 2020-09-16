---
title: 2419-không thể-để-bật-kiểm tra
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767621"
---
# <a name="unable-to-enable-unified-auditing"></a>Không thể bật kiểm định hợp nhất

Khi bạn cố gắng bật kiểm tra hợp nhất cho tổ chức của mình, bạn có thể nhận được lỗi tương tự như sau:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Để giải quyết vấn đề này, hãy làm theo các bước sau đây:

1. [Kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Chạy lệnh ghép ngắn sau đây:

   ```
   Enable-OrganizationCustomization
   ```

3. Hãy chờ 60 phút để cài đặt trước đó có hiệu lực.

4. Chạy lệnh sau đây trong Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Để biết thêm thông tin, hãy xem các bài viết sau đây:

- [Kết nối với Exchange Online PowerShell bằng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Bật hoặc tắt tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
