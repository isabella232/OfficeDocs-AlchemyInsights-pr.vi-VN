---
title: Thiếu email trong cách ly
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892069"
---
# <a name="missing-emails-in-quarantine"></a>Thiếu email trong cách ly

Người quản trị có [thể xem, phát hành hoặc xóa bỏ những thông báo này](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi đến Xem lại **cách** \> **ly**. Hoặc để đi trực tiếp đến **trang Cách ly,** hãy dùng <https://security.microsoft.com/quarantine> .  

Để biết thêm thông tin về các giá trị tìm kiếm/lọc mà bạn có thể dùng, hãy xem Quản lý thư và tệp được cách ly với tư cách là người quản [trị trong EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Lệnh ghép ngắn mà bạn dùng để xem và quản lý thư và tệp trong khu vực cách ly là:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Lưu ý rằng lệnh ghép ngắn này chỉ dành cho thư, không phải là các tệp từ Két sắt attachments cho SharePoint, OneDrive hoặc Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
