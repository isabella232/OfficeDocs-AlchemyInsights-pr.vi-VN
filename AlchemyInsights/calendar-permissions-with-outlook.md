---
title: Quyền lịch
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862162"
---
# <a name="calendar-permissions"></a>Quyền lịch

Người dùng có thể thay đổi quyền lịch của riêng mình với Outlook trên web hoặc các máy khách khác, nhưng là quản trị viên mà bạn có thể cần điều tra là tốt.  
Với lệnh ghép ngắn Exchange PowerShell sẽ hiển thị cho bạn quyền trên lịch của người dùng:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Để xem thêm thông tin, hãy xem mục sau:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Thiết lập MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Thêm MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Quyền lịch được sử dụng trong việc chia sẻ lịch, để xem thêm thông tin về chia sẻ lịch Outlook, hãy xem các bài viết này:

- [Chia sẻ lịch Outlook với người khác](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Chia sẻ lịch của bạn trong Outlook trên web cho doanh nghiệp](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Để khắc phục sự cho phép lịch bạn có thể sử dụng công cụ [hỗ trợ và trợ lý phục hồi](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .