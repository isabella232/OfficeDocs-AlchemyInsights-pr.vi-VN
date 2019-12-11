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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959516"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook không thể kết nối với thư mục công cộng

Nếu truy cập thư mục công cộng không hoạt động cho một số người dùng, hãy thử như sau:

Kết nối với EXO PowerShell và đặt cấu hình DefaultPublicFolderMailbox trên tài khoản người dùng sự cố để phù hợp với một tài khoản người dùng đang hoạt động.

Ví dụ:

Get-Mailbox Workingngười dùng | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-hộp thư ProblemUser-DefaultPublicFolderMailbox \<giá trị từ lệnh trước>

Hãy đợi ít nhất một giờ để thay đổi có hiệu lực.