---
title: Thêm nhóm vào một trang web SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770373"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Vấn đề khi tạo một nhóm kết nối trang web trong SharePoint

1. Một số vấn đề phổ biến gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.
Nếu bạn đã xóa một nhóm và trang web được kết nối của nó và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần xóa vĩnh viễn trang web trước đó.

   - Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Để biết thêm thông tin về việc bắt đầu với PowerShell, xem bắt [đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Loại bỏ các trang web khỏi xóa các trang web bằng cách sử dụng lệnh ghép ngắn PowerShell [loại bỏ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell là bắt buộc để xóa vĩnh viễn các trang web nhóm.

1. Nếu bạn đang tạo trang web được kết nối nhóm và nhận cảnh báo: **một nhóm khác có cùng bí danh đã tồn tại**, hãy kiểm tra các nhóm hiện có từ [Office 365 từ Trung tâm quản trị](https://admin.microsoft.com/AdminPortal/Home#/groups). Để khắc phục sự cố, xoá nhóm hiện có nếu nó không còn cần thiết hoặc tạo ra các trang web với một bí danh khác được chỉ định.

1. Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.

   - Bạn có thể kết nối các trang web hiện tại với một nhóm Office 365. Để biết thêm thông tin, hãy xem [kết nối nhóm Office 365 bằng cách sử dụng giao diện người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Để tạo một trang web nhóm Office 365 được kết nối, bạn sẽ cần tạo một [site nhóm](https://admin.microsoft.com/sharepoint).
