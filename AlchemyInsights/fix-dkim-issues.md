---
title: Khắc phục sự cố thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945953"
---
# <a name="fix-dkim-setup-issues"></a>Khắc phục sự cố thiết lập DKIM

Nếu bạn gặp sự cố khi bật DKIM cho tên miền riêng của mình, hãy sử dụng các bước sau đây:

- Hầu hết các sự cố thiết lập DKIM liên quan đến bản ghi DNS không chính xác. Xác minh bản ghi CNAME DKIM **(không phải** bản ghi TXT) được định dạng chính xác. Để biết thêm thông tin, hãy xem chủ [đề này.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Sau khi bạn tạo hoặc cập nhật bản ghi DNS DKIM của mình tại dịch vụ lưu trữ DNS cho miền của mình (thường là nhà đăng ký tên miền), hãy chờ các bản ghi DNS phát hành.

- Nếu bạn không thể tạo các bản ghi DNS DKIM trong trung tâm quản trị, bạn có thể thay thế bằng tên miền riêng của mình (ví dụ: contoso.com) và chạy lệnh \<CustomDomain\> [này trong Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
