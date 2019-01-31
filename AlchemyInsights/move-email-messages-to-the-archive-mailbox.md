---
title: Di chuyển thư vào hộp thư lưu trữ
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660405"
---
Có vấn đề về lưu trữ các mục sang hộp thư lưu trữ. Đảm bảo rằng bạn đã thực hiện các bước sau:
  
1. Xác nhận rằng một **lưu trữ hộp thư** đã được kích hoạt. Nếu không, hãy làm theo bước trong [bài viết này](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) để kích hoạt hộp thư lưu trữ. 
    
2. Trong Trung tâm quản trị Exchange, chọn **Thẻ lưu giữ** quyền **Quản lý tuân thủ**, tạo **thẻ lưu giữ** với các hành động **di chuyển vào lưu trữ** có mong muốn **Thời gian lưu giữ**.
    
3. Trong Trung tâm quản trị Exchange, chọn **Chính sách lưu giữ**, tạo ra một **Chính sách lưu giữ** và thêm của bạn **di chuyển vào lưu trữ** thẻ lưu giữ với chính sách đó. 
    
4. [Gán chính sách lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư người dùng cụ thể. Chính sách tương tự sẽ được áp dụng cho cả **chính** và hộp thư **lưu trữ** . 
    
Hộp thư của người dùng bây giờ cần phải có một chính sách lưu trữ để di chuyển các mục sang hộp thư lưu trữ. Nó có thể là cần thiết để lực lượng quản lý thư mục chương trình hỗ trợ (MFA) chạy và áp dụng các thiết đặt mới cho hộp thư của người dùng. Chạy lệnh sau đây trong khi [kết nối với EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) để bắt đầu các quản lý thư mục chương trình hỗ trợ cho một hộp thư cụ thể: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Muốn biết thêm thông tin về việc thiết lập một chính sách lưu trữ, hãy xem [thiết lập một chính sách lưu trữ và xóa hộp thư](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

