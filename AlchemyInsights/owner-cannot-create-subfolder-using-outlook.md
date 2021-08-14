---
title: Chủ sở hữu không thể tạo thư mục con bằng cách Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063146"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Chủ sở hữu không thể tạo thư mục con bằng cách Outlook

**Hiện đang xảy ra sự cố với chủ sở hữu thư mục công cộng khi tạo thư mục con bằng Outlook. Sự cố này sẽ sớm được khắc phục.**

Trong khi đó, hãy sử dụng một trong các giải pháp thay thế sau:

1. Sử Outlook cho MAC để tạo thư mục con khi sự cố chỉ ảnh hưởng tới các cửa sổ Outlook dành cho máy tính để bàn (tất cả các phiên bản)
2. Để người quản trị tạo thư mục con bằng EXO Shell hoặc EAC
3. Thay đổi DefaultPublicFolderMailbox/EffectivePublicFolderMailbox trên người dùng sang hộp thư khác ngoài Hộp thư Nội dung cho thư mục gây ra sự cố  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Chờ một giờ, khởi động lại máy khách outlook