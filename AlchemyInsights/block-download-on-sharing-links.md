---
title: Chặn tải xuống trên các nối kết chia sẻ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685764"
---
# <a name="block-download-on-sharing-links"></a>Chặn tải xuống trên các nối kết chia sẻ

**Chặn tải xuống** có sẵn cho các **nối kết chỉ xem** đến tài liệu Office. Khi bạn chọn tùy chọn này, những người được quyền truy nhập vào tệp thông qua liên kết bạn đã tạo sẽ không thấy các tùy chọn để tải xuống, in hoặc sao chép tệp.

Người quản trị có thể kiểm soát việc cài đặt "chặn tải xuống" chỉ xuất hiện đối với các tệp Office hay không bằng cách thay đổi `BlockDownloadLinksFileType` thiết đặt trong các lệnh ghép ngắn [Set-chắp](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) hoặc [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
