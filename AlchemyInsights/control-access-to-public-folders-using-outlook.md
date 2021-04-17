---
title: Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816762"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kiểm soát quyền truy nhập vào các thư mục công cộng bằng Outlook

Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook:

1. Sử dụng `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook  
$false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook. Đây là giá trị mặc định.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Lưu ý: quy trình này chỉ có thể điều khiển kết nối với Outlook trên máy tính cho máy khách chạy Windows. Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.

Để biết thêm thông tin, hãy xem [kiểm soát kết nối đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf) để biết thêm thông tin.
