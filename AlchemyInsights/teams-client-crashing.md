---
title: Đội khách hàng bị rơi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354076"
---
# <a name="teams-client-crashing"></a>Đội khách hàng bị rơi?

Nếu khách hàng teams của bạn bị sập, hãy thử các cách sau:

- Nếu bạn đang sử dụng ứng dụng teams trên máy tính để bàn, hãy đảm [bảo rằng ứng dụng được Cập Nhật hoàn toàn](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Đảm bảo rằng tất cả các [URL của Microsoft 365 và phạm vi địa chỉ](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy cập.

- Đăng nhập bằng tài khoản quản trị viên của bạn và kiểm tra [bảng điều khiển dịch vụ y tế](https://docs.microsoft.com/office365/enterprise/view-service-health) để xác minh rằng không có sự cố hỏng hóc hoặc dịch vụ tồn tại.

- Gỡ cài đặt và cài đặt lại ứng dụng teams (liên kết)
    - Duyệt đến thư mục%appdata%\Microsoft\teams\ trên máy tính của bạn và xoá tất cả các tệp trong thư mục đó.
    - [Tải xuống và cài đặt ứng dụng teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)và nếu có thể, hãy cài đặt teams làm quản trị viên (nhấp chuột phải vào trình cài đặt teams và chọn "chạy với tư vị người quản trị" nếu có).

Nếu khách hàng teams của bạn vẫn bị sập, bạn có thể tạo lại sự cố không? Nếu có:

1. Sử dụng trình ghi bước để nắm bắt các bước của bạn.
    - Đóng tất cả các ứng dụng không cần thiết hoặc bí mật.
    - Khởi động trình ghi bước và tái tạo sự cố khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.
    - [Thu thập các đội ghi mà nắm bắt các bước Create ghi lại](https://docs.microsoft.com/microsoftteams/log-files). **Lưu ý**: đảm bảo bạn chụp địa chỉ đăng nhập của người dùng bị ảnh hưởng.
    - Thu thập các bãi chứa và/hoặc thông tin Xô lỗi (Windows). Khởi chạy Windows PowerShell trên máy mà sự cố xảy ra và chạy các lệnh sau:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Đính kèm tập tin vào trường hợp hỗ trợ của bạn.
