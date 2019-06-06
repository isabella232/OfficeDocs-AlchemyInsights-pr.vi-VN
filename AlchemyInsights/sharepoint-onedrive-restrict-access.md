---
title: Hạn chế truy cập trong SharePoint hoặc OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735164"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế truy cập trong SharePoint hoặc OneDrive

Có rất nhiều cách để hạn chế truy cập vào các dịch vụ SharePoint Online/OneDrive. Những phương pháp hạn chế truy cập khác nhau được trình bày dưới đây. 

Quyền hạn chế

Trong trực tuyến SharePoint và OneDrive cho doanh nghiệp, chúng tôi giới hạn truy cập vào các mục như các trang web, tập tin và thư mục bằng cách chỉ cấp quyền truy cập vào các nhóm/cá nhân nên có thể truy cập.

[Tùy chỉnh cấp phép cho một danh sách SharePoint hoặc thư viện](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Tùy chỉnh cho phép trang web SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Thay đổi quyền truy cập vào một thư mục con](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Điều khiển truy cập từ các thiết bị không được quản lý](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

SharePoint hoặc quản trị toàn cầu trong Office 365, bạn có thể chặn hoặc hạn chế quyền truy cập vào nội dung SharePoint và OneDrive từ các thiết bị không được quản lý (những người không kết hợp quảng cáo tham gia hoặc tuân thủ trong dành).

Giới hạn vị trí mạng

Như là quản trị viên CNTT, bạn có thể kiểm soát quyền truy cập vào tài nguyên SharePoint và OneDrive dựa trên vị trí xác định mạng mà bạn tin tưởng. Điều này cũng được gọi là chính sách dựa trên vị trí. Để biết thêm chi tiết, xin vui lòng xem [kiểm soát quyền truy cập vào dữ liệu OneDrive dựa trên vị trí mạng và SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Trang web Lock hạn chế 

Trong SharePoint Online, bạn có khả năng khóa xuống một bộ sưu tập trang web, do đó, không ai có quyền truy cập. Điều này được thiết lập qua PowerShell và [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng cách sử dụng [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState tài sản.

Hạn chế người dùng từ việc tạo ra trang web này hoặc SubSite

Như là một quản trị SharePoint hoặc Office 365 quản trị toàn cầu, bạn có thể cho phép người dùng tạo và quản lý các trang web SharePoint của riêng họ, xác định những loại trang web, họ có thể tạo ra, và xác định vị trí các trang web. Để biết thêm chi tiết, hãy xem [quản lý tạo ra trang web trong SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

