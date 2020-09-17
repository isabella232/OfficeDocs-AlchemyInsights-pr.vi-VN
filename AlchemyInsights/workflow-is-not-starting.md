---
title: Không bắt đầu dòng công việc
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794789"
---
# <a name="workflow-is-not-starting"></a>Không bắt đầu dòng công việc

- Dòng công việc SharePoint 2010 và dòng công việc SharePoint 2013 không bắt đầu.

    - Nếu dòng công việc của bạn không bắt đầu, có thể có sự cố dịch vụ tạm thời mà người dùng có thể gặp phải sự chậm trễ với dòng công việc. Kiểm tra [bảng điều khiển trạng thái dịch vụ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.

    - Nếu đã trôi qua 24 giờ kể từ lần đầu tiên bạn gặp sự cố này, vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất một giải pháp.

- Dòng công việc SharePoint 2010 bị trì hoãn khi bắt đầu.

    - Điều này xảy ra nếu dòng công việc được kích hoạt trong lô lớn. (ví dụ, khi một số mục được thêm vào một lần).

    - Dòng công việc không được thiết kế để chạy theo thời gian thực, do đó, một hành vi chậm trễ là do thiết kế.

   -  Nếu dòng công việc được mở rộng phức tạp là ngôn ngữ đánh dấu đối tượng (XMOL), thì bạn có thể làm chậm trình tổng hợp. Kiểm tra bài viết [này](https://support.microsoft.com//kb/3043697) .

    - Bạn nên đơn giản hóa dòng công việc hoặc thiết kế lại bằng cách dùng loại nền tảng dòng công việc Microsoft SharePoint 2013.

    - Nếu lịch sử dòng công việc của bạn đã trưởng thành lớn, bạn có thể muốn tẩy các mục hoặc tạo danh sách lịch sử mới.

        Thông tin thêm: [dọn sạch lịch sử](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/) dòng công việc


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo dòng](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


