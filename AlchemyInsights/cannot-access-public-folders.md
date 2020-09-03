---
title: Không thể truy nhập thư mục công cộng
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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341425"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook không thể kết nối với các thư mục công cộng

Nếu quyền truy nhập thư mục công cộng không hoạt động với một số người dùng, hãy thử làm như sau:

Kết nối với EXO PowerShell và đặt cấu hình tham số DefaultPublicFolderMailbox trên tài khoản người dùng vấn đề để khớp với tham số trên tài khoản người dùng đang làm việc.

Mẫu

Hộp thư Get-WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-ProblemUser Mailbox-DefaultPublicFolderMailbox \<value from previous command>

Hãy chờ ít nhất một giờ để thay đổi có hiệu lực.

Nếu vẫn là vấn đề, vui lòng làm theo [quy trình này](https://aka.ms/pfcte) để khắc phục sự cố truy nhập thư mục công cộng bằng cách dùng Outlook.
 
**Để điều khiển người dùng có thể truy nhập vào các thư mục công cộng bằng cách dùng Outlook**:

1.  Sử dụng Set-CASMailbox <mailboxname> -publicfolderclientaccess $True hoặc $false  
      
    $true: cho phép người dùng truy nhập các thư mục công cộng trong Outlook  
      
    $false: ngăn chặn quyền truy nhập của người dùng vào các thư mục công cộng trong Outlook. Đây là giá trị mặc định.  
        
2.  Thiết lập tổ chức-trình cài đặt cấu hình-kiểm soát $true   
      
**Ghi chú** Quy trình này chỉ có thể kiểm soát các kết nối với Outlook trên máy tính cho máy khách chạy Windows. Người dùng có thể tiếp tục truy nhập vào các thư mục công cộng bằng OWA hoặc Outlook for Mac.
 
Để biết thêm thông tin, hãy xem thông [báo hỗ trợ các kết nối được kiểm soát đến các thư mục công cộng trong Outlook](https://aka.ms/controlpf).