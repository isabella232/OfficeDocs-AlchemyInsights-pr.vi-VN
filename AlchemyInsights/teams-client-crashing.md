---
title: Teams máy khách gặp sự cố
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890360"
---
# <a name="teams-client-crashing"></a>Teams máy khách gặp sự cố

Nếu máy khách Teams gặp sự cố, hãy thử cách sau:

- Nếu bạn đang sử dụng ứng Teams trên máy tính, hãy [đảm bảo ứng dụng được cập nhật đầy đủ.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

- Hãy đảm bảo rằng tất [cả các URL Microsoft 365 và dải địa chỉ đều](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy nhập được.

- Đăng nhập bằng tài khoản [](https://docs.microsoft.com/office365/enterprise/view-service-health) người quản trị đối tượng thuê của bạn và kiểm tra Bảng điều khiển Tình trạng Dịch vụ của bạn để xác nhận rằng không tồn tại sự cố hoặc giảm dịch vụ.

- Gỡ cài đặt và cài đặt lại Teams Application
    - Duyệt đến thư mục %appdata%\Microsoft\Teams\ trên máy tính của bạn, rồi xóa tất cả các tệp trong thư mục đó.
    - Tải [xuống và cài đặt Ứng dụng Teams](https://www.microsoft.com/microsoft-teams/download-app)và nếu có thể, hãy cài đặt Teams người  quản trị (bấm chuột phải vào chương trình cài đặt Teams, rồi chọn Chạy với tư cách người quản trị, nếu có).

Nếu máy khách Teams gặp sự cố, hãy tìm cách tái tạo sự cố. Nếu bạn có thể:

1. Sử dụng Trình ghi Bước để ghi lại các bước của bạn.
    - Đóng TẤT CẢ các ứng dụng không cần thiết hoặc bảo mật.
    - Khởi chạy Trình ghi Bước và tái tạo sự cố khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.
    - [Thu thập nhật ký nhóm ghi lại các bước tiến hành lại được ghi lại.](https://docs.microsoft.com/microsoftteams/log-files) **Lưu** ý : Đảm bảo bạn ghi lại được địa chỉ đăng nhập của người dùng bị ảnh hưởng.
    - Thu thập thông tin về việc kết xuất và/hoặc Bộ chứa lỗi (Windows). Khởi Windows Powershell trên máy đang xảy ra sự cố và chạy các lệnh sau (sau mỗi lệnh, hãy nhấn Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Sau khi tạo tệp văn bản và xuất hiện trên màn hình của bạn, hãy lưu tệp và đính kèm tệp vào yêu cầu dịch vụ. 
