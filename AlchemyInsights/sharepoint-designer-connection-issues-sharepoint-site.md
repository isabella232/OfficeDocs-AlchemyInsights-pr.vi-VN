---
title: Cấp phép SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760714"
---
# <a name="sharepoint-designer-connection-issues"></a>Vấn đề kết nối SharePoint Designer 

Nếu SharePoint Designer gặp phải vấn đề kết nối với các trang web SharePoint, xin vui lòng thử các giải pháp phổ biến sau.

Bước 1: Xác minh SharePoint Designer được Cập Nhật.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Cập Nhật cho SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Bước 2: Xóa các tập tin bộ đệm ẩn cục bộ

- Đóng SharePoint Designer 2013.

- Trên máy tính địa phương, trình duyệt các thư mục sau đây để loại bỏ các tập tin lưu trữ.

- Click vào Start, Run và xóa tất cả các tập tin được tìm thấy dưới mỗi của các bên dưới vị trí.

Máy chủ %AppData%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Mở SharePoint Designer 2013 và nhập vào tài khoản một lần nữa để xem nếu nó hoạt động.

Bước 3: Cho [phép xác thực hiện đại cho Office 2013 trên cửa sổ thiết bị](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Bước 4: Quản trị viên sẽ cần phải cho phép tuỳ chỉnh Script cho phép kết nối SharePoint Designer.

Bước chi tiết, ví dụ và cân nhắc xem [cho phép hoặc ngăn chặn các tuỳ chỉnh script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


