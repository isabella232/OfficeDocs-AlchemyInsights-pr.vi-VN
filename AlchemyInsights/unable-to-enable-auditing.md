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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="19a67-102">Không thể để cho phép kiểm tra thống nhất</span><span class="sxs-lookup"><span data-stu-id="19a67-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="19a67-103">Khi bạn cố gắng để cho phép kiểm toán thống nhất cho các tổ chức Office 365 của bạn, bạn có thể nhận được lỗi tương tự như sau:</span><span class="sxs-lookup"><span data-stu-id="19a67-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="19a67-104">Để giải quyết vấn đề này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="19a67-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="19a67-105">[Kết nối để trao đổi trực tuyến Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="19a67-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="19a67-106">Chạy lệnh sau đây:</span><span class="sxs-lookup"><span data-stu-id="19a67-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="19a67-107">Chờ 60 phút cho các thiết lập trước đó có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="19a67-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="19a67-108">Hãy chạy lệnh sau trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="19a67-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="19a67-109">Để biết thêm chi tiết, xem các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="19a67-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="19a67-110">Kết nối với Exchange Online PowerShell sử dụng nhiều yếu tố xác thực</span><span class="sxs-lookup"><span data-stu-id="19a67-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="19a67-111">Bật Office 365 kiểm toán đăng nhập tìm hoặc tắt</span><span class="sxs-lookup"><span data-stu-id="19a67-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
