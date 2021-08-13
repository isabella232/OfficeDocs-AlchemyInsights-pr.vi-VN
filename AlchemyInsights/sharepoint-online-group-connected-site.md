---
title: Thêm nhóm vào một SharePoint site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093825"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Các vấn đề thường gặp khi tạo một site được kết nối nhóm trong SharePoint

1. Nếu bạn đã xóa một nhóm và site được kết nối của nhóm đó và muốn tạo một site khác có cùng URL, bạn sẽ cần phải loại bỏ vĩnh viễn site trước đó.

   - Tải [xuống SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Để biết thêm thông tin về việc bắt đầu với Powershell, [xem mục Bắt đầu với SharePoint Online Management Shell.](/powershell/module/sharepoint-online/remove-sposite)
   - Loại bỏ Site khỏi các Site đã Xóa bằng lệnh ghép ngắn [Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Cần có Powershell để xóa vĩnh viễn các site nhóm.

1. Nếu bạn đang tạo một nhóm được kết nối site và nhận được một cảnh **báo:** Một nhóm khác có cùng biệt danh đã tồn tại , hãy kiểm tra các nhóm hiện có [từ Trung tâm quản trị Microsoft 365.](https://admin.microsoft.com/AdminPortal/Home#/groups) Để giải quyết vấn đề này, hãy xóa nhóm hiện có nếu nhóm đó không còn cần thiết hoặc tạo site với một biệt danh khác được gán.

1. Có nhiều cách khác nhau để tạo và sử dụng nhóm hiện đại với SharePoint.

   - Bạn có thể kết nối các site hiện có với Microsoft 365 nhóm. Để biết thêm thông tin, [hãy Kết nối nhóm Microsoft 365 sử dụng giao diện SharePoint dùng chính](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Để tạo một Microsoft 365 kết nối site, bạn sẽ cần tạo một [Site Nhóm.](https://admin.microsoft.com/sharepoint)
