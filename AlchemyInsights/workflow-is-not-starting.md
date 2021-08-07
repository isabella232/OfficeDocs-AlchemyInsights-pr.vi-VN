---
title: Dòng công việc không bắt đầu
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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907760"
---
# <a name="workflow-is-not-starting"></a>Dòng công việc không bắt đầu

- SharePoint việc 2010 SharePoint 2013 và 2013 không bắt đầu.

    - Nếu dòng công việc của bạn không bắt đầu, có thể là một vấn đề dịch vụ tạm thời trong đó người dùng có thể gặp phải sự chậm trễ không liên tục với tiến độ dòng công việc. Kiểm tra Bảng [điều khiển Tình trạng Dịch](https://admin.microsoft.com/AdminPortal/Home/servicehealth) vụ để xem liệu tổ chức của bạn có bị ảnh hưởng không.

    - Nếu hơn 24 giờ trôi qua kể từ khi bạn gặp sự cố này lần đầu tiên, vui lòng ghi nhật ký thẻ hỗ trợ. Trong nhiều trường hợp, chúng tôi đang nỗ lực tìm giải pháp. Vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất giải pháp.

- SharePoint việc 2010 bị trì hoãn khi bắt đầu.

    - Điều này xảy ra nếu dòng công việc được kích hoạt trong các lô lớn. (ví dụ, khi thêm một vài mục cùng lúc).

    - Dòng công việc không được thiết kế để chạy theo thời gian thực, vì vậy độ trễ là hành vi theo thiết kế.

   -  Nếu Dòng công việc là ngôn ngữ đánh dấu đối tượng có thể chia thành phức tạp (XMOL), việc biên soạn có thể chậm. Hãy xem [bài viết](https://support.microsoft.com//kb/3043697) này.

    - Bạn nên đơn giản hóa dòng công việc hoặc thiết kế lại dòng công việc bằng cách sử dụng kiểu nền tảng Dòng công việc Microsoft SharePoint 2013.

    - Nếu lịch sử dòng công việc của bạn đã phát triển lớn, bạn có thể muốn dọn sạch các mục hoặc tạo một danh sách lịch sử mới.

        Thông tin Khác: Dọn [sạch Lịch sử Dòng công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow thực hiện SharePoint Online?
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
