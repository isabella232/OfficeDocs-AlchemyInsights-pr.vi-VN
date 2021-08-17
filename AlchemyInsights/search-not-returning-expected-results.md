---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052732"
---
# <a name="content-search-not-returning-expected-results"></a>Tìm kiếm Nội dung không trả về kết quả mong đợi

Khi chạy Tìm kiếm Nội dung từ Trung tâm Microsoft 365 mật & Chính của Mình, bạn có thể nhận được kết quả tìm kiếm không mong muốn. Hãy cân nhắc những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:

- **Vị trí nội dung và điều kiện tìm kiếm:** Hãy đảm bảo bạn đã chọn vị trí nội dung và điều kiện tìm kiếm phù hợp. Nếu bạn đã chạy một tìm kiếm lớn (có nhiều vị trí), hãy cân nhắc việc tách tìm kiếm thành nhiều tìm kiếm.

- **Các mục được lập chỉ mục một phần:**  [Các mục được lập chỉ mục một phần](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) từ hộp thư được đưa vào kết quả tìm kiếm ước tính. Tuy nhiên, các mục được lập chỉ mục một phần từ các SharePoint và OneDrive sẽ không được đưa vào giá trị ước tính tìm kiếm.

- Lỗi **tìm** kiếm: Khi tìm kiếm một lượng lớn hộp thư (hơn 100.000 hộp thư), bạn có thể gặp lỗi tìm kiếm, kèm theo mã lỗi như CS008-009 và CS012-002). Trong trường hợp này, hãy chỉ tìm kiếm lại cho vị trí nội dung không thành công. Hãy xem  [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) để biết thêm thông tin.
