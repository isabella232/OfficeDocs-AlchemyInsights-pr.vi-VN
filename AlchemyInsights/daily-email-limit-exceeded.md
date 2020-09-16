---
title: Vượt quá giới hạn email hàng ngày. Dòng công việc bị tạm ngừng.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731585"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Vượt quá giới hạn email hàng ngày. Dòng công việc bị tạm ngừng.

Lỗi này có thể nhận được trong những tình huống sau đây:

- Bạn có dòng công việc trong SharePoint Online vốn đang dùng kiểu nền tảng SharePoint 2010 hoặc SharePoint 2013 dòng công việc.
- Dòng công việc được cấu hình để gửi thông điệp email tùy chỉnh cho hơn 200 người dùng cùng lúc, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.
- Khi bạn chạy dòng công việc, thông điệp email không được gửi đi và bạn nhận thấy hành vi sau đây:
    - Đối với dòng công việc bằng cách dùng loại nền tảng SharePoint 2013, bạn duyệt đến trang **trạng thái** dòng công việc. Trên trang trạng thái dòng công việc, **trạng thái nội bộ** được đặt thành **bắt đầu**và bóng chú thích sẽ hiển thị **không thể gửi cho người nhận**.

Để giải quyết vấn đề này, hãy cấu hình dòng công việc của bạn để gửi thư email mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Ví dụ: sử dụng tạm dừng trong dòng công việc, gửi email đến một nhóm Microsoft 365, nhóm phân phối hoặc nhóm bảo mật cho phép thư hoặc gửi thư đến ít hơn 200 người nhận mỗi lần.


Để biết thêm thông tin, hãy xem [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)sau đây.

## <a name="related-topics"></a>Chủ đề liên quan
- [Tạo dòng](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng](https://flow.microsoft.com/blog/sharepoint-and-flow/) 