---
title: Khắc phục sự cố thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506796"
---
# <a name="fix-dkim-setup-issues"></a>Khắc phục sự cố thiết lập DKIM

Nếu bạn gặp sự cố cho phép DKIM cho miền tuỳ chỉnh của bạn, sử dụng các bước sau:

- Hầu hết các sự cố thiết lập DKIM có liên quan đến bản ghi DNS không chính xác. Kiểm tra bản ghi DKIM CNAME (**không** phải bản ghi TXT) được định dạng chính xác. Để biết thêm thông tin, xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)này.

- Sau khi bạn tạo hoặc Cập Nhật bản ghi DKIM DNS của mình tại dịch vụ lưu trữ DNS cho miền của bạn (thông thường, công ty đăng ký tên miền của bạn), hãy đợi bản ghi DNS truyền.

- Nếu bạn không thể tạo bản ghi DKIM DNS trong Trung tâm quản trị, bạn có thể thay thế \<CustomDomain\> bằng miền tuỳ chỉnh của bạn (ví dụ: contoso.com) và chạy lệnh này trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
