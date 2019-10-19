---
title: Hạn chế quyền truy cập trong SharePoint hoặc OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750686"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế quyền truy cập trong SharePoint hoặc OneDrive

Có nhiều cách để hạn chế quyền truy cập vào dịch vụ SharePoint Online/OneDrive. Các phương pháp hạn chế truy cập khác nhau được nêu dưới đây. 

**Hạn chế quyền**

Trong SharePoint Online và OneDrive for Business, chúng tôi giới hạn quyền truy cập vào các mục như trang web, tệp và thư mục bằng cách chỉ cấp quyền truy cập vào các nhóm/cá nhân có quyền truy cập.

- [Tuỳ chỉnh quyền cho một danh sách SharePoint hoặc thư viện](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tùy chỉnh quyền trang web SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Thay đổi quyền trên một thư mục con](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kiểm soát truy cập từ các thiết bị không quản lý](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Là một SharePoint hoặc quản trị toàn cầu trong Office 365, bạn có thể chặn hoặc giới hạn truy cập vào SharePoint và OneDrive nội dung từ thiết bị không được quản lý (những người không kết hợp AD tham gia hoặc phù hợp trong InTune).

**Giới hạn vị trí mạng**

Là quản trị viên CNTT, bạn có thể kiểm soát quyền truy cập vào tài nguyên SharePoint và OneDrive dựa trên các vị trí mạng được xác định mà bạn tin cậy. Điều này còn được gọi là chính sách dựa trên vị trí. Để biết thêm thông tin, hãy xem [kiểm soát truy cập vào dữ liệu SharePoint trực tuyến và OneDrive dựa trên vị trí mạng](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Hạn chế khóa trang web** 

Trong SharePoint Online, bạn có khả năng khóa một bộ sưu tập trang web, do đó, không ai có quyền truy cập. Điều này được thiết lập qua PowerShell và [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng cách sử dụng thuộc tính [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Hạn chế người dùng tạo trang web hoặc trang web con**

Là một quản trị SharePoint hoặc quản trị viên toàn cầu Office 365, bạn có thể cho phép người dùng của bạn tạo và quản lý các trang web SharePoint của riêng họ, xác định loại trang web mà họ có thể tạo và chỉ định vị trí của các trang web. Để biết thêm thông tin, hãy xem [quản lý tạo trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

