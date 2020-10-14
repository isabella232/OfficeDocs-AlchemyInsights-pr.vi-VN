---
title: Thư mục được phép gửi dưới dạng thư công cộng trong EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462078"
---
# <a name="sendas-mail-enabled-public-folder"></a>Thư mục công cộng được kích hoạt trong SendAs mail

Ví dụ sau đây gán quyền "gửi dưới dạng" cho thư mục công cộng cho phép thư NewPF1 đến Jason của người dùng.

Add-RecipientPermission-Identity ' NewPF1 '-Trustee "Jason"-AccessRights ' SendAs '

Để biết thông tin về cú pháp và tham số chi tiết, hãy xem [gán quyền "gửi dưới dạng" hoặc "gửi thay mặt" cho các thư mục công cộng cho phép thư](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

