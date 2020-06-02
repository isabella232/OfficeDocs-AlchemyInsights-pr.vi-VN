---
title: 2419-không thể kích hoạt kiểm tra
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510450"
---
# <a name="unable-to-enable-unified-auditing"></a>Không thể cho phép kiểm tra hợp nhất

Khi bạn cố gắng kích hoạt kiểm tra hợp nhất cho tổ chức của bạn, bạn có thể nhận được lỗi tương tự như sau:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Để khắc phục sự cố này, hãy làm theo các bước sau:

1. [Kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Chạy lệnh sau:

   ```
   Enable-OrganizationCustomization
   ```

3. Đợi 60 phút cho cài đặt trước có hiệu lực.

4. Chạy lệnh sau trong Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Để biết thêm thông tin, hãy xem bài viết sau đây:

- [Kết nối với Exchange Online PowerShell sử dụng xác thực nhiều yếu tố](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Bật hoặc tắt tìm kiếm Nhật ký kiểm tra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
