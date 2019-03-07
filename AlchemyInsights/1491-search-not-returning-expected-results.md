---
title: 1491-Search-not-Returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29965001"
---
# <a name="content-search-not-returning-expected-results"></a>Tìm kiếm nội dung không phải trả lại kết quả mong đợi

Khi chạy nội dung tìm kiếm từ Office 365 an ninh & Trung tâm phù hợp, bạn có thể nhận được kết quả tìm kiếm không mong muốn. Hãy xem xét những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:

- **Vị trí nội dung và các điều kiện tìm kiếm**: đảm bảo rằng bạn đã lựa chọn địa điểm thích hợp của nội dung và điều kiện tìm kiếm. Nếu bạn chạy một tìm kiếm lớn (với nhiều địa điểm), xem xét việc chia tách nó thành nhiều tìm kiếm.

- **Một phần được lập chỉ mục các mục**: [một phần được lập chỉ mục các mục](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) khỏi hộp thư được bao gồm trong kết quả tìm kiếm ước tính. Tuy nhiên, các khoản mục được đánh chỉ mục một phần từ các trang web trong SharePoint và OneDrive không được bao gồm trong các ước tính tìm kiếm.

- **Tìm kiếm thất bại**: khi tìm kiếm một số lượng lớn các hộp thư (hộp thư trên 100.000), bạn có thể nhận được lỗi tìm, với mã lỗi chẳng hạn như CS008-009 và CS012-002). Trong trường hợp này, thử lại tìm kiếm chỉ cho các vị trí nội dung đã thất bại. Xem [bài viết này](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) để biết thêm thông tin.