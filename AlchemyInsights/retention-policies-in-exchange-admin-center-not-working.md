---
title: Chính sách lưu giữ trong Exchange trung tâm quản trị không làm việc
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935014"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Chính sách lưu giữ trong Trung tâm quản trị Exchange

 **Vấn đề:** Vừa được tạo ra hoặc Cập Nhật duy trì chính sách trong Trung tâm quản trị Exchange không áp dụng cho hộp thư hoặc mục không được chuyển đến hộp thư lưu trữ hoặc xóa bỏ. 
  
 **Nguyên nhân gốc rễ:**
  
- Điều này có thể là do sự **Quản lý thư mục chương trình hỗ trợ** đã không xử lý hộp thư của người dùng. Chương trình hỗ trợ thư mục quản lý cố xử lý từng thư trong tổ chức dựa trên đám mây của bạn một lần mỗi bảy ngày. Nếu bạn thay đổi thẻ lưu giữ hoặc áp dụng một chính sách lưu giữ khác cho một hộp thư, bạn có thể đợi cho đến khi người quản lý thư mục hỗ trợ xử lý hộp thư, hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant để bắt đầu các quản lý thư mục chương trình hỗ trợ xử lý cụ thể hộp thư. Chạy lệnh ghép ngắn này là hữu ích để thử hay gỡ rối một chính sách lưu giữ hoặc cài đặt thẻ lưu giữ. Để biết thêm chi tiết, truy cập vào [chạy chương trình hỗ trợ thư mục quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Giải pháp:** Chạy lệnh sau để bắt đầu các quản lý thư mục chương trình hỗ trợ cho một hộp thư cụ thể: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Này cũng có thể xảy ra nếu **RetentionHold** đã là **kích hoạt** trong hộp thư. Nếu hộp thư đã được đặt trên một RetentionHold, chính sách lưu giữ trên hộp thư sẽ không được xử lý trong thời gian đó. Cho thêm informaton vào xem cài đặt RetentionHold: [Hộp thư lưu trữ tổ chức](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Giải pháp:**
    
  - Kiểm tra tình trạng của các thiết lập RetentionHold trong hộp thư cụ thể trong [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Hãy chạy lệnh sau để **vô hiệu hóa** RetentionHold trên một hộp thư cụ thể: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Bây giờ, chạy lại các thư mục được quản lý trợ lý:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, chương trình hỗ trợ thư mục quản lý sẽ không tự động xử lý hộp thư. 
  

