---
title: Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700477"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế quyền truy nhập trong SharePoint hoặc OneDrive

Có nhiều cách để hạn chế quyền truy nhập vào các dịch vụ SharePoint Online/OneDrive. Những phương pháp hạn chế truy nhập khác nhau được nêu dưới đây. 

**Hạn chế cấp phép**

Trong SharePoint Online và OneDrive for Business, chúng tôi giới hạn quyền truy nhập vào các mục như site, tệp và thư mục bằng cách chỉ cấp quyền truy nhập vào các nhóm/cá nhân cần có quyền truy nhập.

- [Tùy chỉnh quyền đối với danh sách hoặc thư viện SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tùy chỉnh quyền đối với site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Thay đổi quyền trên thư mục con](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kiểm soát truy nhập từ thiết bị không được quản lý](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Với tư cách là người quản trị SharePoint hoặc toàn cầu, bạn có thể chặn hoặc giới hạn quyền truy nhập vào SharePoint và OneDrive từ các thiết bị không được quản lý (không kết hợp với quảng cáo được gia nhập hoặc tuân thủ trong InTune).

**Giới hạn vị trí mạng**

Với tư cách là người quản trị CNTT, bạn có thể kiểm soát quyền truy nhập vào các tài nguyên SharePoint và OneDrive dựa trên vị trí mạng được xác định bạn tin tưởng. Điều này còn được gọi là chính sách dựa trên vị trí. Để biết thêm thông tin, vui lòng xem [kiểm soát quyền truy nhập vào dữ liệu SharePoint Online và OneDrive dựa trên vị trí mạng](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Giới hạn khóa của site** 

Trong SharePoint Online, bạn có khả năng khóa một tuyển tập trang, vì vậy không ai có quyền truy nhập. Điều này được đặt thông qua PowerShell và [Shell quản lý SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng thuộc tính [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Hạn chế người dùng tạo site hoặc trang phụ**

Với tư cách là người quản trị SharePoint hoặc người quản trị toàn cầu, bạn có thể cho phép người dùng của mình tạo và quản lý các site SharePoint riêng của họ, xác định loại site nào mà họ có thể tạo và xác định vị trí của các site. Để biết thêm thông tin, vui lòng xem [quản lý việc tạo site trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

