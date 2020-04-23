---
title: Khắc phục sự cố sử dụng mở với Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759714"
---
# <a name="fix-problems-with-open-with-explorer"></a>Khắc phục sự cố với Open With Explorer

Khắc phục sự cố thường gặp với việc mở thư viện tài liệu trong SharePoint hoặc OneDrive bằng lệnh **mở Explorer** : 
  
- Sử dụng Internet Explorer 10 hoặc Internet Explorer 11. **Mở bằng Explorer** không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác. **Mở với Explorer** bị vô hiệu hoá trong tất cả các trình duyệt ngoại trừ Internet Explorer. 
    
- **Mở bằng Explorer** không có trong trải nghiệm hiện đại cho thư viện SharePoint. Sử dụng **dạng xem trong file Explorer** thay thế. Chọn xem **tùy chọn** \> **xem trong file Explorer**. Xem trong file Explorer không tương thích với Microsoft Edge, Google Chrome, Firefox và những người khác. **Xem trong file Explorer** chỉ có sẵn trong Internet Explorer. 
    
- Đảm bảo rằng dịch vụ WebClient đang chạy. Trong hộp tìm kiếm của Windows, nhập chạy, chọn ứng dụng Run Desktop, gõ Services. msc, và sau đó nhấn Enter. Cuộn xuống dịch vụ WebClient và đảm bảo rằng cột **trạng thái** Hiển thị "đang chạy." Nếu không, bấm đúp vào dịch vụ, bấm **bắt đầu**, và sau đó bấm **OK**. (Bạn có thể cần phải kích hoạt dịch vụ trước tiên bằng cách chọn **hướng dẫn sử dụng** hoặc **tự động** trong hộp **loại khởi động** .) 
    
> [!NOTE]
> Mở một thư viện trong file Explorer là tiện dụng nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần, nhưng nếu bạn muốn thường xuyên làm việc trong thư viện, chúng tôi khuyên bạn nên đồng bộ hóa nó. Để khắc phục sự cố mở trong file Explorer, hãy xem [mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Để biết thông tin về thiết lập đồng bộ hóa, [hãy xem đồng bộ hóa tệp SharePoint với khách hàng đồng bộ OneDrive mới](https://go.microsoft.com/fwlink/?linkid=871666).
  
Vui lòng xem bài viết [cách sử dụng lệnh "mở bằng Explorer" để khắc phục sự cố trong SharePoint trực tuyến để](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) biết thêm thông tin. 
  

