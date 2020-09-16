---
title: Chính sách duy trì trong Trung tâm quản trị Exchange không hoạt động
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740532"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Chính sách duy trì trong Trung tâm quản trị Exchange

Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các thiết đặt được đề cập dưới đây, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của người dùng có vấn đề với chính sách duy trì.

 **Vấn đề:** Các chính sách duy trì mới được tạo hoặc Cập Nhật trong Trung tâm quản trị Exchange không áp dụng cho các hộp thư hoặc mục sẽ không được di chuyển đến hộp thư lưu trữ hoặc bị xóa. 
  
 **Nguyên nhân gốc:**
  
- Điều này có thể do **trợ lý thư mục được quản lý** không xử lý hộp thư của người dùng. Trợ lý thư mục được quản lý cố gắng xử lý tất cả các hộp thư trong tổ chức dựa trên nền tảng điện toán đám mây của bạn một lần mỗi bảy ngày. Nếu bạn thay đổi thẻ duy trì hoặc áp dụng chính sách duy trì khác vào hộp thư, bạn có thể đợi cho đến khi thư mục được quản lý hỗ trợ quy trình hộp thư hoặc bạn có thể chạy lệnh ghép ngắn Start-ManagedFolderAssistant để bắt đầu bộ trợ giúp thư mục được quản lý để xử lý một hộp thư cụ thể. Chạy lệnh ghép ngắn này rất hữu ích cho việc thử nghiệm hoặc khắc phục sự cố các thiết đặt thẻ duy trì hoặc chính sách duy trì. Để biết thêm thông tin, hãy truy cập [chạy trình trợ giúp thư mục được quản lý](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Giải pháp:** Chạy lệnh sau đây để bắt đầu trợ lý thư mục được quản lý cho một hộp thư cụ thể:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Điều này cũng có thể xảy ra nếu **RetentionHold** đã được **kích hoạt** trên hộp thư. Nếu hộp thư đã được đặt trên một RetentionHold, chính sách duy trì trên hộp thư sẽ không được xử lý trong thời gian đó. Để biết thêm thông tin chi tiết về cài đặt RetentionHold, hãy xem: [giữ duy trì hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Nghiệm**
    
  - Kiểm tra trạng thái của thiết đặt RetentionHold trên hộp thư cụ thể trong [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Chạy lệnh sau đây để **vô hiệu hóa** RetentionHold trên một hộp thư cụ thể:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Bây giờ, hãy chạy lại trợ lý thư mục được quản lý:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, trợ lý thư mục được quản lý sẽ không tự động xử lý hộp thư.
 
Để biết thêm thông tin về chính sách duy trì trong Trung tâm quản trị Exchange, hãy xem:
- [Thẻ duy trì và chính sách duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Áp dụng chính sách duy trì cho hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Thêm hoặc loại bỏ thẻ duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Cách xác định loại giữ được đặt trên một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
