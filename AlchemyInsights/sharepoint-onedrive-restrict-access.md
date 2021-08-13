---
title: Hạn chế truy nhập trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093912"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế truy nhập trong SharePoint hoặc OneDrive

Có nhiều cách để hạn chế truy nhập vào các dịch SharePoint Online/OneDrive khác. Các phương pháp hạn chế truy nhập khác nhau này được nêu dưới đây. 

**Hạn chế Quyền**

Trong SharePoint Online và OneDrive for Business, chúng tôi hạn chế quyền truy nhập vào các mục như site, tệp và thư mục chỉ bằng cách cấp quyền truy nhập vào các nhóm/cá nhân sẽ có quyền truy nhập.

- [Tùy chỉnh quyền cho danh sách SharePoint thư viện](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Tùy chỉnh SharePoint quyền site](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Thay đổi quyền trên một thư mục con](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kiểm soát quyền truy nhập từ những thiết bị không được quản lý](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Với tư cách là người quản trị SharePoint hoặc người quản trị toàn cầu, bạn có thể chặn hoặc giới hạn quyền truy nhập vào nội dung SharePoint và OneDrive từ các thiết bị không được quản lý (những thiết bị không kết hợp AD được liên kết hoặc tuân thủ trong Intune).

**Hạn chế Vị trí Mạng**

Với tư cách là người quản trị CNTT, bạn có thể kiểm soát quyền truy nhập vào SharePoint và OneDrive tài nguyên dựa trên vị trí mạng được xác định mà bạn tin cậy. Điều này còn được gọi là chính sách dựa trên vị trí. Để biết thêm thông tin, vui lòng [xem mục Kiểm soát quyền truy SharePoint Dữ liệu OneDrive Online dựa trên vị trí mạng](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Hạn chế khóa site** 

Trong SharePoint Online, bạn có thể khóa tuyển tập site vì vậy không ai có quyền truy nhập. Điều này được đặt thông qua PowerShell và [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) bằng thuộc tính [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Hạn chế người dùng tạo site hoặc site con**

Với tư cách là người quản trị SharePoint hoặc Người quản trị toàn cầu, bạn có thể cho phép người dùng tạo và quản trị các site SharePoint của riêng mình, xác định loại site họ có thể tạo và xác định vị trí của các site. Để biết thêm thông tin, vui lòng [xem Quản lý việc tạo site SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

