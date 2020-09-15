---
title: Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665740"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Chủ sở hữu không thể tạo thư mục con bằng cách dùng Outlook

**Có vấn đề liên tiếp với chủ sở hữu thư mục công cộng tạo thư mục con bằng cách dùng Outlook. Vấn đề sẽ sớm được khắc phục.**

Trong khi đó, hãy dùng một trong các giải pháp thay thế sau đây:

1. Sử dụng Outlook for MAC để tạo thư mục con là sự cố chỉ tác động đến Windows for Desktop (Tất cả các phiên bản)
2. Quản trị tạo thư mục con bằng EXO Shell hoặc EAC
3. Thay đổi DefaultPublicFolderMailbox/EffectivePublicFolderMailbox trên người dùng đến hộp thư khác ngoài hộp thư nội dung cho thư mục gây ra sự cố  
    - *Set-Mailbox user1 DefaultPublicFolderMailbox PubMBX3*
4. Chờ một giờ, khởi động lại ứng dụng khách Outlook