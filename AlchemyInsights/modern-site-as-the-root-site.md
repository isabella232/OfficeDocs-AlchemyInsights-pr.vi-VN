---
title: Site hiện đại là site gốc
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327624"
---
# <a name="modern-site-as-root-site"></a>Site hiện đại là site gốc

Chúng tôi đã bắt đầu triển khai một tính năng mới sẽ cho phép bạn hoán đổi site gốc [site cổ điển của mình với một site hiện đại.](https://docs.microsoft.com/sharepoint/modern-root-site) Dùng [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của site với một site khác trong khi lưu trữ site gốc. Sẵn dùng cho cả Site Nhóm (không được kết nối với nhóm) và Site Liên lạc.

**Quan trọng:** Không xóa site gốc cổ điển của bạn để tạo Site Liên lạc hiện đại. Điều này không được Microsoft hỗ trợ. Việc xóa site gốc sẽ khiến tất cả các site SharePoint trong tổ chức của bạn không thể truy nhập với tất cả người dùng, cho đến khi bạn khôi phục site hoặc tạo site mới ở cùng một URL. Chúng tôi sẽ liên lạc với tính năng này qua trung tâm thông báo. Bạn sẽ sớm bật tính năng này trong đối tượng thuê của mình.

## <a name="known-issues-with-swapping-sites"></a>Sự cố đã biết với hoán đổi site
- Site đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Cần phải nhận biết nội dung để cập nhật chỉ mục tìm kiếm. Không có bước thủ công nào được yêu cầu ở đây, thao tác này sẽ được thực hiện tự động.
- Mọi thứ phụ thuộc vào nối kết "tĩnh" (chẳng hạn như Đồng bộ Tệp và OneNote) sẽ cần được sửa lại theo cách thủ công.
- Project Có thể các site máy chủ cần được xác thực để đảm bảo rằng chúng vẫn được liên kết đúng. 
