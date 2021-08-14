---
title: SharePoint Các vấn đề về kết nối trong trình thiết kế
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942047"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Các vấn đề về kết nối trong trình thiết kế 

Nếu Trình thiết SharePoint gặp sự cố kết nối với các SharePoint site của mình, vui lòng thử các giải pháp phổ biến sau đây.

Bước 1: Xác minh rằng SharePoint Designer 2013 được cập nhật cùng [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và Bản cập nhật [02/08/2016 cho SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Bước 2: Xóa các tệp bộ đệm ẩn cục bộ:

1. Đóng Trình SharePoint Designer 2013.

2. Trên máy tính cục bộ, loại bỏ tất cả các tệp được tìm thấy trong từng thư mục sau đây.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Mở SharePoint Designer 2013, rồi nhập lại tài khoản để xem liệu tài khoản có hoạt động không.

Bước 3: [Bật Xác thực Hiện đại cho Office 2013 trên thiết Windows mới.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Bước 4: Người quản  trị sẽ cần Cho phép Script Tùy chỉnh trong thiết đặt Trung tâm Quản trị SharePoint cho phép kết nối SharePoint Designer của bạn. Xem mục [Cho phép hoặc ngăn chặn tập lệnh tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) để biết thêm thông tin.


