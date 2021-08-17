---
title: Quyền đối với Lịch
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
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046126"
---
# <a name="calendar-permissions"></a>Quyền đối với Lịch

Người dùng có thể thay đổi Quyền Lịch của riêng mình Outlook trên Web hoặc máy khách khác nhưng với tư cách là người quản trị, bạn có thể cần phải điều tra.  
Với Exchange lệnh ghép ngắn PowerShell sẽ hiển thị cho bạn quyền trên lịch của người dùng:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Để xem thêm thông tin, hãy xem các mục sau:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Quyền Lịch được sử dụng trong việc chia sẻ lịch, để xem thêm thông tin về việc chia sẻ Outlook lịch, hãy xem các bài viết sau đây:

- [Chia sẻ Outlook lịch với người khác](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Chia sẻ lịch của bạn trong Outlook trên web dành cho doanh nghiệp](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Để khắc phục sự cố Quyền Lịch, bạn có thể sử [dụng công Công cụ Trợ giúp Phục hồi và Hỗ trợ](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) công cụ.