---
title: Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804007"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook

Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook:

1. Sử dụng `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook  
$false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook. Đây là giá trị mặc định.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Lưu ý: quy trình này chỉ có thể điều khiển kết nối với Outlook trên máy tính cho máy khách chạy Windows. Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.

Để biết thêm thông tin, hãy xem [kiểm soát kết nối đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf) để biết thêm thông tin.
