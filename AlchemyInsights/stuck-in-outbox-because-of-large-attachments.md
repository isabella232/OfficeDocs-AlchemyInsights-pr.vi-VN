---
title: Bị kẹt trong hộp thư đi vì các tệp đính kèm lớn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232652"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Khắc phục thông báo bị kẹt trong hộp thư đi

Chúng tôi khuyên bạn bắt đầu bằng cách chạy kịch bản ["tôi gặp sự cố khi gửi, nhận hoặc tìm thư email"](https://aka.ms/SaRA-OutlookSendReceive) từ công cụ [Microsoft support và Recovery Assistant](https://diagnostics.office.com/#/) trên máy bị ảnh hưởng.

Khi một thông báo bị kẹt trong hộp thư đi của bạn, nguyên nhân có thể là một phần đính kèm lớn hoặc tùy chọn "gửi ngay lập tức khi kết nối" không được phép.

**Xóa tệp đính kèm lớn**

1. Nhấp vào **gửi/nhận** > **làm việc gián tuyến**. 
2. Trong ngăn điều hướng, nhấp vào **hộp**thư đi. Từ đây, bạn có thể: 
    - Xoùa tin nhaén. Chỉ cần chọn nó và nhấp vào **xóa**.
    - Kéo thư vào **thư mục bản thảo**của bạn, bấm đúp vào để mở thư và xóa phần đính kèm (nhấp vào nó và nhấp vào **xóa**).
3. Nếu lỗi cho bạn biết Outlook đang cố gắng truyền thư, đóng Outlook. Có thể mất vài phút để thoát ra. Nếu Outlook không đóng, nhấn **Ctrl + Alt + Delete** và bấm **bắt đầu trình quản lý tác vụ**. Trong Task Manager, chọn tab **quá trình** , cuộn xuống Outlook. exe, và bấm **kết thúc tiến trình**.
4. Sau khi Outlook đóng, khởi động lại Outlook và lặp lại bước 2-3. 
5. Sau khi bạn loại bỏ các tập tin đính kèm, nhấp vào **gửi/nhận** > **làm việc offline** chọn nút và để tiếp tục làm việc trực tuyến. 

Thông báo cũng gặp khó khăn trong hộp thư đi khi bạn bấm vào **gửi**, nhưng bạn không được kết nối. Nhấp vào **gửi/nhận** và xem nút **làm việc ngoại tuyến** . Nếu màu xanh lam, bạn đã bị ngắt kết nối. Nhấp vào nó để kết nối (nút chuyển sang màu trắng) và nhấp vào **gửi tất cả**.
 
**Cho phép gửi ngay lập tức khi kết nối**
 
1. Trên tab tệp, bấm vào **tuỳ chọn**.

2. Trong hộp thoại Tuỳ chọn Outlook, bấm **nâng cao**.

3. Trong phần gửi và nhận, bấm để cho phép **gửi ngay lập tức khi kết nối**. Bấm **OK**.
 
Để biết chi tiết đầy đủ, xem:
- [Video: gửi hoặc xóa một email bị kẹt](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Email ở cặp hộp thư đi cho đến khi bạn tự bắt đầu hoạt động gửi/nhận trong Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
