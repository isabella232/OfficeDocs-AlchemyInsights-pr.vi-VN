---
title: Tạo một SharePoint site
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
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080912"
---
# <a name="create-a-sharepoint-site"></a>Tạo một SharePoint site

Tạo hoặc quản lý các site từ [các Site Hiện](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) hoạt trong Trung SharePoint tâm Quản trị. Để biết thêm thông tin, [hãy xem mục Quản lý các site trong trung tâm quản SharePoint mới.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>Mẹo:

- Bạn **không** thể tạo site có cùng URL của site hiện có. Nếu bạn đã xóa một site và đang muốn sử dụng lại URL, có thể site đã xóa vẫn tồn tại trong Các site [đã xóa.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) Site sẽ cần bị xóa vĩnh viễn để sử dụng lại URL. Để loại bỏ hoàn toàn site bằng Powershell, hãy xem ví [dụ lệnh ghép ngắn Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Một số người dùng không thể tạo site. [Xem Quản lý việc tạo site trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Có thể site xuất hiện kẹt ở phần Tạo **lâu hơn** dự kiến. Nếu hơn 24 giờ trôi qua kể từ khi bạn gặp sự cố này lần đầu tiên, vui lòng ghi nhật ký thẻ hỗ trợ. Trong nhiều trường hợp, chúng tôi đang nỗ lực tìm giải pháp. Vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất giải pháp.
