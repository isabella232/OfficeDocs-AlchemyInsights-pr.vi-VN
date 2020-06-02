---
title: Chính sách lưu giữ trong Trung tâm quản trị Exchange không hoạt động
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502629"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Chính sách lưu giữ trong Trung tâm quản trị Exchange

 **Vấn đề:** Chính sách mới được tạo hoặc Cập Nhật lưu giữ trong Trung tâm quản trị Exchange không áp dụng cho hộp thư hoặc các mục không được di chuyển vào hộp thư lưu trữ hoặc xoá. 
  
 **Nguyên nhân gốc:**
  
- Điều này có thể do **hỗ trợ thư mục được quản lý** không xử lý hộp thư của người dùng. Hỗ trợ thư mục được quản lý cố gắng xử lý mọi hộp thư trong tổ chức dựa trên ứng dụng web qua Internet của bạn một lần mỗi bảy ngày. Nếu bạn thay đổi thẻ lưu giữ hoặc áp dụng chính sách lưu giữ khác cho hộp thư, bạn có thể đợi cho đến khi quản lý thư mục hỗ trợ quá trình hộp thư, hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant khởi động hỗ trợ thư mục được quản lý để xử lý một hộp thư cụ thể. Chạy lệnh ghép ngắn này rất hữu ích để kiểm tra hoặc khắc phục sự cố cài đặt chính sách lưu giữ hoặc thẻ lưu giữ. Để biết thêm thông tin, hãy truy cập [chạy trình hỗ trợ thư mục được quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Giải pháp:** Chạy lệnh sau để khởi động hỗ trợ thư mục được quản lý cho một hộp thư cụ thể:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Điều này cũng có thể xảy ra nếu **RetentionHold** đã được **kích hoạt** trên hộp thư. Nếu hộp thư đã được đặt trên một RetentionHold, chính sách lưu giữ trên hộp thư sẽ không được xử lý trong thời gian đó. Để biết thêm Informaton trên thiết lập RetentionHold xem: giữ [hộp thư duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Giải pháp:**
    
  - Kiểm tra trạng thái của cài đặt RetentionHold trên hộp thư cụ thể trong [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Chạy lệnh sau để **vô hiệu hoá** RetentionHold trên một hộp thư cụ thể:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Bây giờ, chạy lại hỗ trợ thư mục được quản lý:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Lưu ý:** Nếu hộp thư nhỏ hơn 10 MB, hỗ trợ thư mục được quản lý sẽ không tự động xử lý hộp thư.
 
Để biết thêm thông tin về chính sách lưu giữ trong Trung tâm quản trị Exchange, hãy xem:
- [Chính sách lưu giữ và thẻ lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Áp dụng chính sách lưu giữ cho hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Thêm hoặc xóa thẻ lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Làm thế nào để xác định loại giữ được đặt trên hộp thư](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
