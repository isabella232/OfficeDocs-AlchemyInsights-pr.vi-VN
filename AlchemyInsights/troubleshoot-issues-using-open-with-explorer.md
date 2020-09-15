---
title: Khắc phục sự cố khi mở bằng Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659080"
---
# <a name="fix-problems-with-open-with-explorer"></a>Khắc phục sự cố khi mở với Explorer

Khắc phục các sự cố phổ biến khi mở một thư viện tài liệu trong SharePoint hoặc OneDrive bằng lệnh **mở với Explorer** : 
  
- Sử dụng Internet Explorer 10 hoặc Internet Explorer 11. **Mở với Explorer** không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác. **Mở với Explorer** đã bị vô hiệu hóa trong tất cả các trình duyệt, ngoại trừ Internet Explorer. 
    
- **Mở bằng Explorer** không sẵn dùng trong trải nghiệm hiện đại cho thư viện SharePoint. Sử dụng **dạng xem trong file Explorer** thay vào đó. Chọn dạng xem **tùy chọn xem** \> **trong file Explorer**. Xem trong file Explorer không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác. **Xem trong file Explorer** chỉ sẵn dùng trong Internet Explorer. 
    
- Đảm bảo rằng dịch vụ WebClient đang chạy. Trong hộp tìm kiếm Windows, hãy nhập chạy, chọn ứng dụng chạy trên máy tính, nhập Services. msc, rồi nhấn Enter. Cuộn xuống đến dịch vụ WebClient và đảm bảo cột **trạng thái** sẽ hiển thị "đang chạy". Nếu không, hãy bấm đúp vào dịch vụ, bấm vào **bắt đầu**, rồi bấm **OK**. (Trước tiên, bạn có thể phải bật dịch vụ bằng cách chọn **thủ** công hoặc **tự động** trong hộp **kiểu khởi động** .) 
    
> [!NOTE]
> Mở một thư viện trong file Explorer có ích nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần, nhưng nếu bạn muốn làm việc thường xuyên trong thư viện, chúng tôi khuyên bạn nên đồng bộ nó. Để khắc phục sự cố khi mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Để biết thông tin về việc thiết lập đồng bộ, hãy xem [đồng bộ các tệp SharePoint với máy khách đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).
  
Vui lòng xem bài viết [cách dùng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) để biết thêm thông tin. 
  

