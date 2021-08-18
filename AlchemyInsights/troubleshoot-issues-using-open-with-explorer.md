---
title: Khắc phục sự cố bằng tính năng Mở bằng Explorer
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
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323588"
---
# <a name="fix-problems-with-open-with-explorer"></a>Khắc phục sự cố với Mở bằng Explorer

Khắc phục các sự cố phổ biến khi mở thư viện tài liệu SharePoint hoặc OneDrive cách sử **dụng lệnh Mở bằng Explorer:** 
  
- Sử Internet Explorer 10 hoặc Internet Explorer 11. **Tính năng Mở bằng Explorer** không tương thích với các Microsoft Edge, Google Chrome, Firefox và các ứng dụng khác. **Mở bằng Explorer bị** tắt trong tất cả các trình duyệt ngoại trừ Internet Explorer. 
    
- **Tính năng Mở bằng Explorer** không sẵn dùng trong trải nghiệm hiện đại dành cho các SharePoint khác. Sử **dụng Dạng xem trong File Explorer để thay** thế. Chọn **Xem tùy chọn** Xem trong File \> **Explorer**. Chế độ xem trong File Explorer không tương thích với các Microsoft Edge, Google Chrome, Firefox và các ứng dụng khác. **Xem trong File Explorer** chỉ sẵn dùng trong Internet Explorer. 
    
- Đảm bảo dịch vụ WebClient đang chạy. Trong hộp tìm Windows, nhập Run, chọn ứng dụng Run trên máy tính, nhập services.msc, rồi nhấn Enter. Cuộn xuống dịch vụ WebClient và đảm bảo rằng cột Trạng **thái** hiển thị "Đang chạy". Nếu không, hãy bấm đúp vào dịch vụ, bấm vào **Bắt đầu**, rồi bấm **vào OK.** (Trước tiên, bạn có thể cần phải bật dịch vụ bằng cách chọn Thủ **công** hoặc **Tự động** trong hộp **Loại khởi** động.) 
    
**Lưu** ý: Việc mở thư viện trong File Explorer rất tiện dụng nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần nhưng nếu bạn muốn thường xuyên làm việc trong thư viện, chúng tôi khuyên bạn nên đồng bộ thư viện. Để khắc phục sự cố mở trong File Explorer, hãy [xem Mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Để biết thông tin về cách thiết lập đồng bộ, [hãy xem mục Đồng SharePoint tệp với máy khách Đồng bộ OneDrive mới.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Vui lòng xem bài [viết Cách sử dụng lệnh "Mở bằng Explorer" để khắc](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) phục sự cố trong SharePoint Online để biết thêm thông tin. 
  

