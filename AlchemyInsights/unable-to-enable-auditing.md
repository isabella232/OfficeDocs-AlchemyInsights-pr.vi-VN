---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007812"
---
# <a name="unable-to-enable-unified-auditing"></a>Không thể bật tính năng kiểm tra hợp nhất

Khi bạn cố gắng bật tính năng kiểm tra hợp nhất cho tổ chức của mình, bạn có thể gặp lỗi tương tự như sau:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Để giải quyết vấn đề này, hãy làm theo các bước sau:

1. [Kết nối đổi Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Chạy lệnh ghép ngắn sau đây:

   ```
   Enable-OrganizationCustomization
   ```

3. Chờ 60 phút để cài đặt trước có hiệu lực.

4. Chạy lệnh sau đây Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Để biết thêm thông tin, hãy xem các bài viết sau đây:

- [Kết nối sử Exchange Online PowerShell bằng cách sử dụng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Bật hoặc tắt tìm kiếm nhật ký kiểm tra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
