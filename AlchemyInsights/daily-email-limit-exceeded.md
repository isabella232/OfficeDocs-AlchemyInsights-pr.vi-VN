---
title: Giới hạn email hàng ngày vượt quá. Công việc bị đình chỉ.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059660"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Hàng ngày email vượt quá giới hạn. Công việc bị đình chỉ.

Lỗi này có thể nhận được trong các trường hợp sau:

- Bạn có một công việc trong SharePoint Online, sử dụng SharePoint 2010 hoặc SharePoint 2013 công việc nền tảng loại.
- Các công việc được cấu hình để gửi một tin nhắn tuỳ chỉnh email cho hơn 200 người dùng tại một thời gian, hơn 10.000 người nhận mỗi ngày hoặc nhiều hơn 30 thư mỗi phút.
- Khi bạn chạy quy trình làm việc, thông báo email không được gửi và bạn thông báo các hành vi sau đây:
    - Cho một công việc bằng cách sử dụng các loại nền tảng SharePoint 2013, bạn duyệt đến trang **Tình trạng luồng công việc** . Trên trang tình trạng công việc, **Tình trạng nội bộ** được thiết lập để **bắt đầu**, và hiển thị thông tin bóng **không thể gửi đến người nhận**.

Để làm việc xung quanh vấn đề này, đặt cấu hình công việc của bạn để gửi thư điện tử mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Ví dụ, sử dụng một tạm dừng trong công việc, gửi email cho một nhóm Office 365, một nhóm phân phối hoặc nhóm bảo mật được kích hoạt thư hoặc gửi tin nhắn đến ít hơn 200 người nhận tại một thời điểm.


Để biết thêm chi tiết, xem sau đây [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Chủ đề liên quan
- [Tạo ra dòng chảy](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng chảy](https://flow.microsoft.com/blog/sharepoint-and-flow/) 