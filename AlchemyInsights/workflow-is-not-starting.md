---
title: Công việc không bắt đầu
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558014"
---
# <a name="workflow-is-not-starting"></a>Công việc không bắt đầu

- SharePoint 2010 và SharePoint 2013 quy trình công việc không bắt đầu.

    - Nếu công việc của bạn không bắt đầu, có thể có một vấn đề tạm thời dịch vụ nơi người dùng có thể trải nghiệm sự chậm trễ liên tục với tiến độ công việc. Kiểm tra [Bảng điều khiển dịch vụ y tế](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem nếu tổ chức của bạn bị ảnh hưởng.

    - Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.

- SharePoint 2010 quy trình công việc trì hoãn ngày bắt đầu.

    - Điều này xảy ra nếu các công việc được kích hoạt trong lô lớn. (ví dụ, khi một số khoản mục được thêm vào cùng một lúc).

    - Quy trình công việc không được thiết kế để chạy thời gian thực, do đó, một sự chậm trễ là hành vi của thiết kế.

   -  Nếu công việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), trình biên dịch có thể được làm chậm. Kiểm tra bài viết [này](https://support.microsoft.com/en-us/kb/3043697) .

    - Bạn nên đơn giản hóa các công việc hoặc thiết kế lại nó bằng cách sử dụng các loại nền tảng Microsoft SharePoint 2013 quy trình làm việc.

    - Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các khoản mục hoặc tạo ra một danh sách lịch sử mới.

        Thông tin thêm: [dọn sạch các lịch sử công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Chủ đề liên quan
Bạn muốn thử Microsoft Flow trong SharePoint Online?
- [Tạo ra dòng chảy](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint và dòng chảy](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


