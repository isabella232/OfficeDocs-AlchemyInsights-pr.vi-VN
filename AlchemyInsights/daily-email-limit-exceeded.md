---
title: Vượt quá giới hạn email hàng ngày. Quy trình làm việc bị treo.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908726"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Vượt quá giới hạn email hàng ngày. Quy trình làm việc bị treo.

Lỗi này có thể nhận được trong các trường hợp sau:

- Bạn có một công việc trong SharePoint trực tuyến sử dụng loại nền tảng công việc SharePoint 2010 hoặc SharePoint 2013.
- Luồng công việc được cấu hình để gửi thư email tùy chỉnh cho hơn 200 người dùng tại một thời gian, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.
- Khi bạn chạy luồng công việc, thư email không được gửi và bạn thấy hiện tượng sau:
    - Luồng công việc sử dụng loại nền tảng SharePoint 2013, bạn duyệt trang **trạng thái luồng công việc** . Trên trang trạng thái luồng công việc, **trạng thái nội bộ** được thiết lập để **bắt đầu**, và bóng thông tin hiển thị **không thể gửi đến người nhận**.

Để khắc phục sự cố này, cấu hình luồng công việc của bạn để gửi thư điện tử mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Ví dụ: sử dụng tạm dừng trong quy trình làm việc, gửi email đến một nhóm Microsoft 365, nhóm phân phối hoặc nhóm bảo mật được kích hoạt thư hoặc gửi thư đến ít hơn 200 người nhận tại một thời gian.


Để biết thêm thông tin, hãy xem [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)sau.

## <a name="related-topics"></a>Chủ đề liên quan
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 