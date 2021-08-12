---
title: Đã vượt quá giới hạn email hàng ngày. Dòng công việc bị tạm ngừng.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914673"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Đã vượt quá giới hạn email hàng ngày. Dòng công việc bị tạm ngừng.

Lỗi này có thể xảy ra trong các kịch bản sau đây:

- Bạn có một dòng công việc trong SharePoint Online sử dụng kiểu nền tảng dòng công việc SharePoint 2010 SharePoint 2013.
- Dòng công việc được cấu hình để gửi thư email tùy chỉnh cho hơn 200 người dùng cùng một lúc, hơn 10.000 người nhận mỗi ngày hoặc hơn 30 thư mỗi phút.
- Khi bạn chạy dòng công việc, thông điệp email không được gửi và bạn nhận thấy hành vi sau đây:
    - Đối với dòng công việc sử dụng kiểu SharePoint nền tảng 2013, bạn duyệt đến trang Trạng **thái Dòng công** việc. Trên trang Trạng thái Dòng công việc, Trạng **thái Nội bộ** được đặt thành Bắt đầu và bóng chú thích thông tin hiển thị Không thể gửi đến người **nhận.** 

Để giải quyết vấn đề này, hãy cấu hình dòng công việc của bạn để gửi email mà [không vượt quá giới Exchange Online hạn người gửi.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Ví dụ, hãy dùng một khoảng tạm dừng trong dòng công việc, gửi email đến một nhóm Microsoft 365, một nhóm phân phối hoặc nhóm bảo mật hỗ trợ thư, hoặc gửi thư đến ít hơn 200 người nhận mỗi lần.


Để biết thêm thông tin, hãy xem bài viết [sau đây.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Chủ đề liên quan
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 