---
title: Tạo site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806961"
---
# <a name="create-a-sharepoint-site"></a>Tạo site SharePoint

Tạo hoặc quản lý các site từ [các site hiện hoạt](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) trong Trung tâm quản trị SharePoint. Để biết thêm thông tin, hãy xem [quản lý site trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Ý

- Bạn **không thể** tạo site có cùng một URL của site hiện có. Nếu bạn đã xóa một site và muốn sử dụng lại URL, nó có thể là site đã xóa vẫn tồn tại trong [các site đã xóa](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). Site sẽ cần bị xóa vĩnh viễn để dùng lại URL. Để loại bỏ hoàn toàn một site với PowerShell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .
- Một số người dùng có thể không thể tạo trang. [Xem mục quản lý việc tạo site trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Trang web có thể có vẻ khó khăn khi **tạo** lâu hơn dự kiến. Nếu đã trôi qua 24 giờ kể từ lần đầu tiên bạn gặp sự cố này, vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất một giải pháp.
