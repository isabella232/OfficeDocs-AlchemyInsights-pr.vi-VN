---
title: Thêm một nhóm cho một trang web SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758753"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Tạo nhóm kết nối trang web trong SharePoint Online

Không có một vài vấn đề thường gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.

 Nếu bạn đã xoá một nhóm và trang web được kết nối và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần để vĩnh viễn loại bỏ trang web trước đó.

Tải về [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Để biết thêm chi tiết trên bắt đầu bằng powershell, hãy xem [bắt đầu với SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Loại bỏ các trang web từ xóa các trang web bằng cách sử dụng lệnh ghép ngắn powershell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Nếu bạn đang tạo ra một nhóm kết nối trang web và nhận được một cảnh báo nhóm khác với bí danh cùng đã tồn tại, hãy kiểm tra các nhóm hiện có từ [Office 365 từ Trung tâm quản trị](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Để giải quyết vấn đề, xóa nhóm hiện tại nếu nó không còn cần thiết hoặc tạo ra các trang web với một biệt danh khác nhau được chỉ định.

Có những cách khác nhau để tạo ra và sử dụng các nhóm hiện đại với SharePoint.

Bạn có thể kết nối trang web hiện có với một nhóm Office 365. Để biết thêm chi tiết, hãy xem [kết nối một nhóm Office 365 sử dụng SharePoint người dùng ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Để tạo một trang web được kết nối nhóm Office 365, bạn cần tạo một trang web đội ngũ. Để biết thêm chi tiết, hãy xem [tạo một nhóm trang web trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

