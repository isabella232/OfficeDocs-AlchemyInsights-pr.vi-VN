---
title: Không thể truy cập thư mục công cộng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891771"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook không thể kết nối với thư mục công cộng

Nếu truy cập thư mục công cộng không hoạt động đối với một số người dùng, hãy thử như sau:

Kết nối với EXO PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng sự cố để phù hợp với tham số trên tài khoản người dùng đang hoạt động.

Ví dụ:

Get-Mailbox Workingngười dùng | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-hộp thư ProblemUser-DefaultPublicFolderMailbox \<giá trị từ lệnh trước>

Hãy đợi ít nhất một giờ để thay đổi có hiệu lực.

Nếu sự cố vẫn còn, hãy làm theo [quy trình này](https://aka.ms/pfcte) để khắc phục sự cố truy cập thư mục công cộng bằng cách sử dụng Outlook.