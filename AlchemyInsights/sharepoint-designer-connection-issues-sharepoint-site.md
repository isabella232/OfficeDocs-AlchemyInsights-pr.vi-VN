---
title: Các vấn đề về kết nối của SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727193"
---
# <a name="sharepoint-designer-connection-issues"></a>Các vấn đề về kết nối của SharePoint Designer 

Nếu SharePoint Designer đang gặp vấn đề về kết nối với các site SharePoint, vui lòng thử các giải pháp thông thường sau đây.

Bước 1: xác minh rằng SharePoint Designer 2013 được Cập Nhật với [gói dịch vụ SharePoint Designer 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và bản [Cập Nhật 2 tháng tám 2016 cho SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Bước 2: xóa các tệp bộ đệm ẩn cục bộ:

1. Đóng SharePoint Designer 2013.

2. Trên máy tính cục bộ, hãy loại bỏ tất cả các tệp được tìm thấy trong mỗi thư mục sau đây.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Mở SharePoint Designer 2013 và nhập lại tài khoản để xem liệu nó có hoạt động hay không.

Bước 3: [bật xác thực hiện đại cho Office 2013 trên các thiết bị chạy Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Bước 4: người quản trị sẽ cần cho **phép các tập lệnh tùy chỉnh** trong thiết đặt Trung tâm quản trị SharePoint để cho phép kết nối SharePoint Designer. Xem mục [cho phép hoặc ngăn chặn các tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) để biết thêm thông tin.


