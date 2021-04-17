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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819534"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook không thể kết nối với các thư mục công cộng

Nếu quyền truy nhập thư mục công cộng không hoạt động với một số người dùng, hãy thử làm như sau:

Kết nối với EXO PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng vấn đề để khớp với tham số trên tài khoản người dùng đang làm việc.

Mẫu

Người dùng Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Hãy chờ ít nhất một giờ để thay đổi có hiệu lực.

Nếu vẫn là vấn đề, vui lòng làm theo [quy trình này](https://aka.ms/pfcte) để khắc phục sự cố truy nhập thư mục công cộng bằng cách dùng Outlook.
 
**Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook**:

1.  Sử dụng Set-CASMailbox <mailboxname> -publicfolderaccess $True hoặc $false  
      
    $true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook  
      
    $false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook. Đây là giá trị mặc định.  
        
2.  Các $true Set-OrganizationConfig-Publicfolderđiều khiển   
      
**Ghi chú** Quy trình này chỉ có thể kiểm soát các kết nối với Outlook trên máy tính cho máy khách chạy Windows. Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.
 
Để biết thêm thông tin, hãy xem thông [báo hỗ trợ các kết nối được kiểm soát đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf).