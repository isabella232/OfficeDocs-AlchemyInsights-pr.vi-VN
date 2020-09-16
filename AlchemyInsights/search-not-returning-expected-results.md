---
title: 1491-tìm kiếm-không-trả về-kết quả dự kiến
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740496"
---
# <a name="content-search-not-returning-expected-results"></a>Tìm kiếm nội dung không trả về kết quả dự kiến

Khi chạy các tìm kiếm nội dung từ Trung tâm tuân thủ & bảo mật của Microsoft 365, bạn có thể nhận được kết quả tìm kiếm không mong muốn. Hãy cân nhắc những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:

- **Vị trí nội dung và điều kiện tìm kiếm**: đảm bảo rằng bạn đã chọn các vị trí nội dung thích hợp và các điều kiện tìm kiếm. Nếu bạn đã chạy tìm kiếm lớn (với nhiều vị trí), hãy cân nhắc chia tách nó thành nhiều tìm kiếm.

- Các **mục được lập chỉ mục một phần**: các [mục được lập chỉ mục một phần](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) từ hộp thư được bao gồm trong kết quả tìm kiếm ước tính. Tuy nhiên, các mục được lập chỉ mục một phần từ các site trong SharePoint và OneDrive không được bao gồm trong ước tính tìm kiếm.

- Lỗi **Tìm kiếm**: khi tìm kiếm số lượng hộp thư lớn (trên hộp thư 100.000), bạn có thể gặp lỗi tìm kiếm, với các mã lỗi chẳng hạn như CS008-009 và CS012-002). Trong trường hợp này, hãy thử lại chỉ tìm kiếm cho các vị trí nội dung không thành công. Xem  [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) để biết thêm thông tin.
