---
title: Hạn chế SharePoint Online ở chế độ cổ điển
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958823"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Hạn chế SharePoint Online ở chế độ cổ điển

Một số tổ chức vẫn yêu cầu trải nghiệm chế độ Cổ điển. Mặc dù không có kế hoạch loại bỏ chế độ cổ điển ở mức độ chi tiết nhưng không còn có thể hạn chế toàn bộ tổ chức (đối tượng thuê) sang chế độ cổ điển cho danh sách và thư viện.

Người quản trị sẽ có các tùy chọn sau để quản lý các danh sách và thư viện riêng lẻ ở chế độ cổ điển bằng cách sử dụng các khóa chuyển không tham gia chi tiết mà chúng tôi cung cấp ở các mức sau:

- tuyển tập site
- site
- danh sách
- thư viện

Ngoài ra, danh sách sử dụng một số tính năng và tùy chỉnh nhất định không được hiện đại hỗ trợ vẫn sẽ được tự động chuyển sang chế độ cổ điển.

Bắt đầu từ ngày 1/4/2019, quy trình vô hiệu hóa mức đối tượng thuê để chọn không tham gia vào danh sách hiện đại, các thư viện sẽ bắt đầu và tiếp tục cho đến ngày 31/5/2019.  Các danh sách và thư viện nằm trong chế độ cổ điển do tính năng chọn không tham gia đối tượng thuê sẽ tự động được chuyển sang hiện đại.

Nếu bạn yêu cầu chế [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) độ cổ điển, vui [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) lòng xem thêm thông tin tại đây và hướng dẫn về Powershell PnP ở đây mô tả các tùy chọn và công cụ bạn có thể sử dụng ngay hôm nay để sử dụng trải nghiệm chế độ cổ điển.
