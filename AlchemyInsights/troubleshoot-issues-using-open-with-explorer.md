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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048178"
---
# <a name="fix-problems-with-open-with-explorer"></a>Khắc phục sự cố với Mở bằng Explorer

Khắc phục các sự cố phổ biến khi mở thư viện tài liệu SharePoint hoặc OneDrive cách sử **dụng lệnh Mở bằng Explorer:** 
  
- Sử Internet Explorer 10 Internet Explorer 11. **Tính năng Mở bằng Explorer** không tương thích với các Microsoft Edge, Google Chrome, Firefox và các ứng dụng khác. **Mở bằng Explorer bị** tắt trong tất cả các trình duyệt ngoại trừ Internet Explorer. 
    
- **Tính năng Mở bằng Explorer** không sẵn dùng trong trải nghiệm hiện đại dành cho SharePoint viện. Sử **dụng Dạng xem trong File Explorer để thay** thế. Chọn **Xem tùy chọn** Xem trong File \> **Explorer**. Chế độ xem trong File Explorer không tương thích với các Microsoft Edge, Google Chrome, Firefox và những ứng dụng khác. **Xem trong File Explorer** chỉ sẵn dùng trong Internet Explorer. 
    
- Đảm bảo dịch vụ WebClient đang chạy. Trong hộp tìm Windows, nhập run, chọn ứng dụng Chạy trên máy tính, nhập services.msc, rồi nhấn Enter. Cuộn xuống dịch vụ WebClient và đảm bảo rằng cột Trạng **thái** hiển thị "Đang chạy". Nếu không, hãy bấm đúp vào dịch vụ, bấm vào **Bắt đầu**, rồi bấm **vào OK.** (Trước tiên, bạn có thể cần phải bật dịch vụ bằng cách chọn Thủ **công** hoặc **Tự động** trong hộp **Loại khởi** động.) 
    
> [!NOTE]
> Việc mở thư viện trong File Explorer sẽ rất tiện dụng nếu bạn cần sao chép hoặc di chuyển nhiều tệp và thư mục một lần nhưng nếu bạn muốn thường xuyên làm việc trong thư viện, chúng tôi khuyên bạn nên đồng bộ thư viện. Để khắc phục sự cố mở trong File Explorer, hãy [xem Mở trong Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Để biết thông tin về cách thiết lập đồng bộ, [hãy xem mục Đồng SharePoint tệp với máy khách Đồng bộ OneDrive mới.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Vui lòng xem bài [viết Cách sử dụng lệnh "Mở bằng Explorer" để khắc](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) phục sự cố trong SharePoint Online để biết thêm thông tin. 
  

