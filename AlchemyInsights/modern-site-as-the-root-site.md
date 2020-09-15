---
title: Site hiện đại như site gốc
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666892"
---
# <a name="modern-site-as-root-site"></a>Site hiện đại như site gốc

Chúng tôi đã bắt đầu triển khai một tính năng mới sẽ cho phép bạn [hoán đổi site gốc site cổ điển của bạn với site hiện đại](https://docs.microsoft.com/sharepoint/modern-root-site). Sử dụng cuộc [gọi-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang gốc. Sẵn dùng cho cả site nhóm (không được kết nối với một nhóm) và site liên lạc.

>[!Important]
> Không xóa site gốc cổ điển của bạn để tạo một site liên lạc hiện đại. Điều này không được Microsoft hỗ trợ. Việc xóa site gốc sẽ làm cho tất cả các site SharePoint trong tổ chức của bạn không thể truy nhập được tất cả người dùng, cho đến khi bạn khôi phục site hoặc tạo một site mới tại cùng một URL. Chúng tôi sẽ giao tiếp tính năng này thông qua Trung tâm thông báo. Bạn nên trông đợi tính năng này sẽ được bật trong đối tượng thuê của bạn một thời gian ngắn.

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề đã biết với việc trao đổi site
- Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Nội dung sẽ cần được recrawled để cập nhật chỉ mục tìm kiếm. Không có bước thủ công nào cần thiết ở đây, điều này sẽ được thực hiện tự động.
- Bất kỳ điều gì phụ thuộc vào các nối kết "tĩnh" (chẳng hạn như tệp đồng bộ tệp và tệp OneNote) sẽ cần được sửa chữa theo cách thủ công.
- Các trang web dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết đúng. 
