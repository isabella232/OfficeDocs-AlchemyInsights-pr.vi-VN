---
title: Quyền lịch
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
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819930"
---
# <a name="calendar-permissions"></a>Quyền lịch

Người dùng có thể thay đổi quyền lịch của riêng họ với Outlook trên web hoặc các ứng dụng khách khác, nhưng là người quản trị, bạn có thể cần phải điều tra là tốt.  
Với lệnh ghép ngắn Exchange PowerShell sẽ hiển thị cho bạn quyền trên lịch của người dùng:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Để xem thêm thông tin, hãy xem những điều sau đây:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Thêm-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Quyền lịch được sử dụng trong việc chia sẻ lịch, để xem thêm thông tin về việc chia sẻ lịch Outlook, hãy xem các bài viết sau đây:

- [Chia sẻ lịch Outlook với người khác](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Chia sẻ lịch của bạn trong Outlook trên web dành cho doanh nghiệp](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Để khắc phục sự cố của lịch, bạn có thể sử dụng công cụ [Trợ giúp phục hồi và hỗ trợ](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .