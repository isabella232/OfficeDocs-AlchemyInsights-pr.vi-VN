---
title: Tìm kiếm trong SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044065"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Thu thập dữ liệu nội dung và lập chỉ mục trong SharePoint Online

Nội dung phải được thu thập dữ liệu và thêm vào chỉ mục tìm kiếm để người dùng tìm thấy những gì họ đang tìm kiếm trong SharePoint Online. Nội dung được tự động thu thập thông tin dựa trên lịch chạy dữ liệu được xác định trước (không thể thay đổi lịch thu thập dữ liệu). Trình thu thập thông tin chọn lên nội dung đã thay đổi kể từ lần cuối và Cập Nhật chỉ mục. Để đảm bảo nội dung được thu thập dữ liệu và chỉ mục được Cập Nhật, hãy lưu ý những mục sau:

- Hãy chắc chắn rằng nội dung có thể được tìm thấy bằng cách [làm cho nội dung trang web tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Khi bạn đã thay đổi thuộc tính được quản lý hoặc khi bạn đã thay đổi bản đồ của thuộc tính được quản lý và thu thập dữ liệu, trang web phải được tái thu thập dữ liệu trước khi thay đổi của bạn sẽ được phản ánh trong chỉ mục tìm kiếm. 

    Bởi vì các thay đổi của bạn được thực hiện trong sơ đồ tìm kiếm, và không phải là trang web thực tế, trình thu thập dữ liệu sẽ không tự động tái chỉ mục trang web. 

    Để biết thêm thông tin, xem [yêu cầu thu thập dữ liệu theo cách thủ công và lập chỉ mục lại một trang web, thư viện hoặc danh sách](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Hãy đợi ít nhất 24 giờ sau khi yêu cầu chỉ mục thu thập dữ liệu và toàn bộ lại để xem bạn vẫn gặp sự cố hay chưa. 

    Nếu hơn 24 giờ đã trôi qua kể từ lúc bạn bắt đầu thu thập dữ liệu và chỉ mục lại đầy đủ, vui lòng đăng nhập một trường hợp hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.

> [!IMPORTANT]
> Nếu một trang web, tài liệu (thư viện) hoặc danh sách đã bị xoá và vẫn hiển thị trong kết quả tìm kiếm, người dùng sẽ nhận được **lỗi 404 tệp không tìm thấy** khi cố gắng truy cập. Vấn đề này sẽ được đăng nhập như một trường hợp hỗ trợ để điều tra thêm. 



