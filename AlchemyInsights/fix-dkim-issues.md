---
title: Khắc phục vấn đề thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765549"
---
# <a name="fix-dkim-setup-issues"></a>Khắc phục vấn đề thiết lập DKIM

Nếu bạn gặp vấn đề cho phép DKIM cho miền tuỳ chỉnh của bạn, sử dụng các bước sau:

- Hầu hết các vấn đề thiết lập DKIM có liên quan đến bản ghi DNS không chính xác. Xác minh DKIM bản ghi CNAME (**không phải** bản ghi TXT) được định dạng đúng. Để biết thêm chi tiết, xem [chủ đề](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)này.

- Sau khi bạn tạo hoặc Cập Nhật bản ghi DKIM DNS tại DNS hosting dịch vụ cho tên miền của bạn (thông thường, tên miền đăng ký của bạn), chờ đợi cho các bản ghi DNS để tuyên truyền.

- Nếu bạn không thể tạo DKIM DNS hồ sơ tại Trung tâm quản trị, bạn có thể thay thế \<CustomDomain\> với tên miền riêng của bạn (ví dụ: contoso.com) và chạy lệnh này trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
