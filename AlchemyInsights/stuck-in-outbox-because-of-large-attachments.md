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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441327"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Khắc phục thông báo bị kẹt trong hộp thư đi

Chúng tôi khuyên bạn bắt đầu bằng cách chạy kịch bản ["tôi gặp sự cố khi gửi, nhận hoặc tìm thư email"](https://aka.ms/SaRA-OutlookSendReceive) từ công cụ [hỗ trợ của Microsoft và trợ lý phục hồi](https://diagnostics.office.com/#/) .

Khi một thông báo bị kẹt trong hộp thư đi của bạn, các nguyên nhân có thể là:
- Tệp đính kèm lớn.
- Tùy chọn **gửi ngay khi kết nối** không được kích hoạt.

Để xóa tệp đính kèm lớn: 

1. Trong Outlook, chọn **gửi/nhận** > **làm việc ngoại tuyến**. 
2. Trong ngăn điều hướng, chọn **hộp**thư đi. Từ đây, bạn có thể: 
    - Xoùa tin nhaén (chọn nó và sau đó chọn **Delete**).
    - Kéo thư vào thư mục bản thảo của bạn, bấm đúp để mở nó và xóa phần đính kèm, chọn nó rồi chọn **xóa**).
3. Nếu bạn nhận được lỗi cho biết Outlook đang cố truyền thư, đóng Outlook. Có thể mất vài phút để thoát ra. Nếu Outlook không đóng, nhấn Ctrl + Alt + Delete và chọn **khởi động trình quản lý tác vụ**. Trong Task Manager, chọn tab **quá trình** , cuộn xuống Outlook. exe, và chọn **kết thúc tiến trình**.
4. Sau khi Outlook đóng, khởi động lại và lặp lại bước 2 và 3. 
5. Sau khi bạn loại bỏ phần đính kèm, bấm **gửi/nhận** > **làm việc gián tuyến** để tiếp tục làm việc trực tuyến. 

Thông báo cũng gặp khó khăn trong hộp thư đi khi bạn bấm vào **gửi**, nhưng bạn không được kết nối. Nhấp vào **gửi/nhận** và xem nút **làm việc ngoại tuyến** . Nếu màu xanh lam, bạn đã bị ngắt kết nối. Chọn nó để kết nối (nút chuyển sang màu trắng) và nhấp vào **gửi tất cả**.
 
Để cho phép **gửi ngay lập tức khi kết nối**:
 
- Chọn **tệp** > **tùy chọn** >  **nâng cao**.
Trong phần **gửi và nhận** , chọn **gửi ngay khi được kết nối**, sau đó chọn **OK**.
 
Để biết chi tiết đầy đủ xem:
- [Video: gửi hoặc xóa một email bị kẹt](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Email ở cặp hộp thư đi cho đến khi bạn tự bắt đầu hoạt động gửi/nhận trong Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
