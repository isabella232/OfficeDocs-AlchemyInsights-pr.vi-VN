---
title: Kiểm soát quyền truy nhập vào các thư mục công cộng bằng cách Outlook
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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032580"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kiểm soát quyền truy nhập vào các thư mục công cộng bằng cách Outlook

Để kiểm soát người dùng nào có thể truy nhập thư mục công cộng bằng cách Outlook:

1. Sử dụng `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Cho phép người dùng truy nhập thư mục công cộng trong Outlook  
$false: Ngăn người dùng truy nhập vào thư mục công cộng trong Outlook. Đây là giá trị mặc định.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Lưu ý: Thủ tục này chỉ có thể kiểm soát các kết nối với Outlook bàn làm việc cho máy Windows khách. Người dùng có thể tiếp tục truy nhập thư mục công cộng bằng cách sử dụng OWA Outlook for Mac.

Để biết thêm thông tin, hãy xem [Kết nối có Kiểm soát đến Thư mục Công cộng Outlook](https://aka.ms/controlpf) biết thêm thông tin.
