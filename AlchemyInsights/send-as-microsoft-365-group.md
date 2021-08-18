---
title: Nhóm Gửi với Microsoft 365 Người dự
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
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086150"
---
# <a name="send-as-microsoft-365-group"></a>Nhóm Gửi với Microsoft 365 Người dự

Bạn có thể gán quyền Gửi Dưới tên để cho phép người dùng cụ thể gửi thư dưới dạng Microsoft 365 nhóm:  

1. Kết nối để Exchange Online PowerShell.  

2. Chạy lệnh sau:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Để biết thêm thông tin, [hãy xem Cho phép các thành viên gửi dưới dạng hoặc gửi thay mặt cho một nhóm.](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)