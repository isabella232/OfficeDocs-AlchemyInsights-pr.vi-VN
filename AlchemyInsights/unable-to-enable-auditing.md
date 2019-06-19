---
title: 2419-không-để-enable-kiểm toán
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065729"
---
# <a name="unable-to-enable-unified-auditing"></a>Không thể để cho phép kiểm tra thống nhất

Khi bạn cố gắng để cho phép kiểm toán thống nhất cho các tổ chức Office 365 của bạn, bạn có thể nhận được lỗi tương tự như sau:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Để giải quyết vấn đề này, hãy làm theo các bước sau:

1. [Kết nối để trao đổi trực tuyến Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Chạy lệnh sau đây:

   ```
   Enable-OrganizationCustomization
   ```

3. Chờ 60 phút cho các thiết lập trước đó có hiệu lực.

4. Hãy chạy lệnh sau trong Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Để biết thêm chi tiết, xem các bài viết sau đây:

- [Kết nối với Exchange Online PowerShell sử dụng nhiều yếu tố xác thực](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Bật Office 365 kiểm toán đăng nhập tìm hoặc tắt](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
