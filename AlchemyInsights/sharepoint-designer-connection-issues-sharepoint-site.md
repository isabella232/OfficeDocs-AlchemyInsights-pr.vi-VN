---
title: Vấn đề kết nối SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840573"
---
# <a name="sharepoint-designer-connection-issues"></a>Vấn đề kết nối SharePoint Designer 

Nếu SharePoint Designer gặp phải vấn đề kết nối với các trang web SharePoint, vui lòng thử các giải pháp phổ biến sau.

Bước 1: Xác minh rằng SharePoint Designer 2013 được Cập Nhật với [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) và [2 tháng tám năm 2016 Cập Nhật cho SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Bước 2: Xóa các tập tin bộ đệm ẩn cục bộ:

1. Đóng SharePoint Designer 2013.

2. Trên máy tính, loại bỏ tất cả các file trong mỗi thư mục sau đây được tìm thấy.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Mở SharePoint Designer 2013 và nhập vào tài khoản một lần nữa để xem nếu nó hoạt động.

Bước 3: Cho [phép xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Bước 4: Quản trị viên sẽ cần phải **Cho phép tuỳ chỉnh Script** trong các thiết lập Trung tâm quản trị SharePoint cho phép kết nối SharePoint Designer. Xem [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) cho biết thêm thông tin.


