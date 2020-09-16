---
title: Thêm nhóm vào site SharePoint
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771230"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Các vấn đề khi tạo một site được kết nối nhóm trong SharePoint

1. Một số vấn đề phổ biến gặp phải khi tạo hoặc tạo lại một trang kết nối nhóm.
Nếu bạn đã xóa một nhóm và site được kết nối và muốn tạo một site khác với cùng một URL, bạn sẽ cần loại bỏ vĩnh viễn site trước đó.

   - Tải xuống trình [bao quản lý SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Để biết thêm thông tin về việc bắt đầu với PowerShell, hãy xem [bắt đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Loại bỏ site khỏi các site đã xóa bằng lệnh ghép ngắn PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell được yêu cầu để xóa vĩnh viễn các site nhóm.

1. Nếu bạn đang tạo một trang kết nối nhóm và nhận cảnh báo: **một nhóm khác với cùng một biệt danh đã tồn tại**, hãy kiểm tra các nhóm hiện có từ [Trung tâm quản trị Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Để giải quyết sự cố này, hãy xóa nhóm hiện có nếu nó không còn cần thiết hoặc tạo site có một biệt danh khác được gán.

1. Có nhiều cách khác nhau để tạo và sử dụng các nhóm hiện đại với SharePoint.

   - Bạn có thể kết nối các site hiện có với một nhóm Microsoft 365. Để biết thêm thông tin, hãy xem [kết nối nhóm Microsoft 365 bằng cách sử dụng giao diện người dùng SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Để tạo site Microsoft 365 được kết nối, bạn sẽ cần tạo [site nhóm](https://admin.microsoft.com/sharepoint).
