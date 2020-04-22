---
title: Luồng công việc không bắt đầu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766119"
---
# <a name="workflow-is-not-starting"></a>Luồng công việc không bắt đầu

- SharePoint 2010 và SharePoint 2013 luồng công việc không khởi chạy.

    - Nếu công việc của bạn không khởi động, có thể có sự cố dịch vụ tạm thời mà người dùng có thể gặp phải gián đoạn liên tục với tiến trình luồng công việc. Kiểm tra [bảng điều khiển tình trạng dịch vụ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.

    - Nếu hơn 24 giờ đã trôi qua kể từ lần đầu tiên bạn thấy vấn đề này, vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.

- Luồng công việc SharePoint 2010 chậm trễ trên bắt đầu.

    - Điều này xảy ra nếu công việc được kích hoạt trong lô lớn. (ví dụ: khi một số mục được thêm vào cùng một lúc).

    - Luồng công việc không được thiết kế để chạy thời gian thực, do đó, sự chậm trễ là hành vi thiết kế.

   -  Nếu quy trình làm việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), biên soạn có thể chậm. Kiểm tra bài viết [này](https://support.microsoft.com//kb/3043697) .

    - Bạn nên đơn giản hóa công việc hoặc thiết kế lại nó bằng cách sử dụng loại nền tảng Microsoft SharePoint 2013 luồng công việc.

    - Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các mục hoặc tạo danh sách lịch sử mới.

        Thông tin thêm: [xoá lịch sử luồng công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


