---
title: Gửi dưới dạng Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740173"
---
# <a name="send-as-microsoft-365-group"></a>Gửi dưới dạng Microsoft 365

Bạn có thể gán quyền gửi dưới dạng để cho phép người dùng cụ thể gửi thư dưới dạng nhóm Microsoft 365:  

1. Kết nối với Exchange Online PowerShell.  

2. Chạy lệnh sau:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Để biết thêm thông tin, hãy xem [cho phép các thành viên gửi dưới dạng hoặc gửi thay mặt cho một nhóm](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).