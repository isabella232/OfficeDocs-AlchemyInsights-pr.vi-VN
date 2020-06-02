---
title: Sự cố kết nối SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511566"
---
# <a name="sharepoint-designer-connection-issues"></a>Sự cố kết nối SharePoint Designer 

Nếu SharePoint Designer đang gặp sự cố kết nối với các trang web SharePoint, hãy thử các giải pháp phổ biến sau.

Bước 1: xác minh rằng SharePoint Designer 2013 được Cập Nhật với [SharePoint Designer gói dịch vụ 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và [ngày 2, 2016 Cập Nhật cho SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Bước 2: xóa các tệp bộ đệm ẩn cục bộ:

1. Đóng SharePoint Designer 2013.

2. Trên máy tính cục bộ, loại bỏ tất cả các tệp được tìm thấy trong mỗi thư mục sau đây.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Mở SharePoint Designer 2013 và nhập lại tài khoản để xem nếu nó hoạt động.

Bước 3: [kích hoạt xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Bước 4: quản trị viên sẽ cần phải **cho phép tuỳ chỉnh tập lệnh** trong cài đặt Trung tâm quản trị SharePoint cho phép kết nối SharePoint Designer. Xem cho [phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) để biết thêm thông tin.


