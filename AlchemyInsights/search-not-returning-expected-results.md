---
title: 1491-tìm kiếm-không-trở lại-dự kiến-kết quả
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510594"
---
# <a name="content-search-not-returning-expected-results"></a>Tìm kiếm nội dung không trả lại kết quả mong đợi

Khi chạy tìm kiếm nội dung từ Microsoft 365 bảo mật & Trung tâm tuân thủ, bạn có thể nhận được kết quả tìm kiếm không mong muốn. Hãy xem xét những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:

- **Vị trí nội dung và điều kiện tìm kiếm**: đảm bảo bạn đã chọn vị trí nội dung phù hợp và điều kiện tìm kiếm. Nếu bạn chạy một tìm kiếm lớn (với nhiều vị trí), hãy xem xét chia tách nó thành nhiều tìm kiếm.

- **Mục đã lập chỉ mục một**phần: các [mục đã lập chỉ mục một phần](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) từ hộp thư được bao gồm trong kết quả tìm kiếm ước tính. Tuy nhiên, một phần được lập chỉ mục từ các trang web trong SharePoint và OneDrive không được bao gồm trong ước tính tìm kiếm.

- Lỗi **Tìm kiếm**: khi tìm kiếm một số lượng lớn hộp thư (trên 100.000 hộp thư), bạn có thể nhận được lỗi tìm kiếm, với mã lỗi như CS008-009 và CS012-002). Trong trường hợp này, thử tìm kiếm chỉ cho các vị trí nội dung không thành công. Xem [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) để biết thêm thông tin.
