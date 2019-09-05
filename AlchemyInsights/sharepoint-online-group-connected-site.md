---
title: Thêm nhóm vào một trang web SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750542"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Vấn đề khi tạo hoặc nhóm các trang web được kết nối trong SharePoint trực tuyến

Có một vài vấn đề phổ biến gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.

 Nếu bạn đã xóa một nhóm và trang web được kết nối của nó và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần xóa vĩnh viễn trang web trước đó.

Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Để biết thêm thông tin về việc bắt đầu với PowerShell, xem bắt [đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Loại bỏ các trang web khỏi xóa các trang web bằng cách sử dụng lệnh ghép ngắn PowerShell [loại bỏ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Nếu bạn đang tạo một nhóm kết nối trang web và nhận được cảnh báo một nhóm khác với cùng một bí danh đã tồn tại, kiểm tra các nhóm hiện có từ [Office 365 từ Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Để khắc phục sự cố, xoá nhóm hiện có nếu nó không còn cần thiết hoặc tạo ra các trang web với một bí danh khác được chỉ định.

Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.

Bạn có thể kết nối các trang web hiện tại với một nhóm Office 365. Để biết thêm thông tin, hãy xem [kết nối một nhóm Office 365 bằng cách sử dụng ineterface người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Để tạo một trang web nhóm Office 365 được kết nối, bạn sẽ cần tạo một site nhóm. Để biết thêm thông tin, xem [tạo trang web nhóm trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

