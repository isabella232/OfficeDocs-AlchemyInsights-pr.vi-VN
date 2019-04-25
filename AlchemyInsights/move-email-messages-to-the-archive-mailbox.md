---
title: Di chuyển thư vào hộp thư lưu trữ
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418347"
---
# <a name="move-email-to-the-archive-mailbox"></a>Di chuyển email sang hộp thư lưu trữ
 
1. Xác nhận rằng một **lưu trữ hộp thư** đã được kích hoạt. Nếu không, sử dụng các bước trong [bài viết này](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) để kích hoạt hộp thư lưu trữ.

2. Lưu trữ tin nhắn tự động cho hộp thư lưu trữ, thẻ lưu giữ với hành động **di chuyển vào lưu trữ** phải được đặt để **áp dụng tự động cho từ khóa toàn bộ hộp thư (mặc định)**. Sử dụng các bước dưới đây để tạo ra các từ khóa: [lưu trữ mặc định từ khóa](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Tiếp theo, thêm **lưu trữ** thẻ chính sách lưu giữ của bạn. Trong Trung tâm quản trị Exchange, chọn **Chính sách lưu giữ** > thêm **di chuyển vào lưu trữ thẻ** cho > chính sách **tiết kiệm**. 
    
4. Bây giờ [chỉ định chính sách lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư người dùng cụ thể. Chính sách tương tự sẽ được áp dụng cho cả **chính** và hộp thư **lưu trữ** . 
    
Nó có thể là cần thiết để lực lượng quản lý thư mục chương trình hỗ trợ (MFA) chạy và áp dụng các thiết đặt mới cho hộp thư của người dùng. Chạy lệnh sau đây trong khi [kết nối với EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) để bắt đầu các quản lý thư mục chương trình hỗ trợ cho một hộp thư cụ thể: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Để biết thêm chi tiết về thiết lập một chính sách lưu trữ, hãy xem [thiết lập một chính sách lưu trữ và xóa hộp thư](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

