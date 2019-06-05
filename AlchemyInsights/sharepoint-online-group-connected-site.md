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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719503"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Tạo nhóm kết nối trang web trong SharePoint Online

<p><strong>Không có một vài vấn đề thường gặp phải khi tạo hoặc tái tạo một nhóm kết nối trang web.&nbsp;</strong></p>  <p>1.Nếu bạn đã xoá một nhóm và trang web được kết nối và muốn tạo một trang web khác với cùng một URL, bạn sẽ cần để vĩnh viễn loại bỏ trang web trước đó.</p>  <ul>  <li>Tải về <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - để biết thêm thông tin về bắt đầu với powershell, hãy xem <a title="bắt đầu với SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Bắt đầu với SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Loại bỏ các trang web bằng cách xóa bỏ các trang web sử dụng các <a title="hủy bỏ-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Hủy bỏ-SPODeletedSite</a> lệnh ghép ngắn powershell.</li>  </ul>  <p>Nếu bạn đang tạo ra một nhóm kết nối trang web và nhận được một cảnh báo <strong>'nhóm khác với bí danh cùng đã tồn tại'</strong>, hãy kiểm tra các nhóm hiện có từ các <a title="Office 365 từ Trung tâm quản trị" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 từ Trung tâm quản trị</a>. Để giải quyết vấn đề, xóa nhóm hiện tại nếu nó không còn cần thiết hoặc tạo ra các trang web với một biệt danh khác nhau được chỉ định.&nbsp;</p>  <p><strong>Có những cách khác nhau để tạo ra và sử dụng các nhóm hiện đại với SharePoint.&nbsp;</strong></p>  <ol>  <li>Bạn có thể kết nối trang web hiện có với một nhóm Office 365. Để biết thêm thông tin, hãy xem <a title="kết nối một nhóm Office 365 sử dụng SharePoint người dùng ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Kết nối một nhóm Office 365 sử dụng SharePoint người dùng ineterface</a>.</li>  <li>Để tạo một trang web được kết nối nhóm Office 365, bạn cần tạo một trang web đội ngũ. Để biết thêm thông tin, hãy xem <a title="tạo ra một nhóm trang web trong SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Tạo ra một nhóm trang web trong SharePoint.</a></li>  </ol>

