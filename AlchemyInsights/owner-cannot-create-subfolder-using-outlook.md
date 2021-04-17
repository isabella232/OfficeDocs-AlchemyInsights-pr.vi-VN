---
title: Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836157"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook

**Có vấn đề liên tiếp với chủ sở hữu thư mục công cộng tạo thư mục con bằng cách dùng Outlook. Vấn đề sẽ sớm được khắc phục.**

Trong khi đó, hãy dùng một trong các giải pháp thay thế sau đây:

1. Sử dụng Outlook for MAC để tạo thư mục con là sự cố chỉ tác động đến Windows for Desktop (Tất cả các phiên bản)
2. Quản trị tạo thư mục con bằng EXO Shell hoặc EAC
3. Thay đổi DefaultPublicFolderMailbox/EffectivePublicFolderMailbox trên người dùng đến hộp thư khác ngoài hộp thư nội dung cho thư mục gây ra sự cố  
    - *Set-Mailbox user1 DefaultPublicFolderMailbox PubMBX3*
4. Chờ một giờ, khởi động lại ứng dụng khách Outlook