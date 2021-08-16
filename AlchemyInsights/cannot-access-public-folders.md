---
title: Không thể truy nhập thư mục công cộng
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996652"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook thể kết nối với thư mục công cộng

Nếu quyền truy nhập thư mục công cộng không hoạt động đối với một số người dùng, hãy thử cách sau:

Kết nối exo PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng sự cố để khớp với tham số trên tài khoản người dùng đang hoạt động.

Ví dụ:

Get-Mailbox workingUser trong | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox problemUser -DefaultPublicFolderMailbox \<value from previous command>

Hãy chờ ít nhất một giờ để thay đổi có hiệu lực.

Nếu sự cố vẫn tiếp tục xảy ra, vui lòng làm theo [quy trình này để](https://aka.ms/pfcte) khắc phục sự cố truy nhập thư mục công cộng Outlook.
 
**Để kiểm soát người dùng nào có thể truy nhập thư mục công cộng bằng cách Outlook:**

1.  Dùng Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true hoặc $false  
      
    $true: Cho phép người dùng truy nhập thư mục công cộng trong Outlook  
      
    $false: Ngăn người dùng truy nhập vào thư mục công cộng trong Outlook. Đây là giá trị mặc định.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Lưu ý** Quy trình này có thể kiểm soát các kết nối chỉ với Outlook bàn làm việc cho máy Windows khách. Người dùng có thể tiếp tục truy nhập thư mục công cộng bằng OWA hoặc Outlook for Mac.
 
Để biết thêm thông tin, hãy [xem Thông báo Hỗ trợ kết nối có kiểm soát đến thư mục công cộng Outlook.](https://aka.ms/controlpf)