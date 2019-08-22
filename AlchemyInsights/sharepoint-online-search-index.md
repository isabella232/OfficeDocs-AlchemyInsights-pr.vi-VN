---
title: Tìm kiếm trong SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507653"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Nội dung thu thập dữ liệu và lập chỉ mục trong SharePoint Online

Nội dung phải được thu thập và bổ sung vào danh mục tìm kiếm cho người dùng tìm thấy những gì họ đang tìm kiếm trong SharePoint Online. Nội dung được tự động thu thập thông tin dựa theo một lịch trình thu thập dữ liệu được xác định trước (lịch trình thu thập thông tin không thể được thay đổi). Thu thập công cụ chọn lên nội dung đã thay đổi kể từ khi thu thập dữ liệu cuối cùng và Cập Nhật chỉ số. Để đảm bảo nội dung thu thập thông tin và chỉ số được Cập Nhật, lưu ý những điều sau đây:

- Đảm bảo rằng nội dung có thể được tìm thấy bằng [cách tìm kiếm nội dung trang web](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Khi bạn đã thay đổi một tài sản được quản lý, hoặc khi bạn đã thay đổi bản đồ của thu thập và quản lý tài sản, các trang web phải được tái crawled trước khi thay đổi của bạn sẽ được phản ánh trong chỉ mục tìm kiếm. 

    Bởi vì các thay đổi được thực hiện trong lược đồ tìm kiếm, và không để các trang web thực tế, các trình thu thập sẽ không tự động tái index trang web. 

    Để biết thêm chi tiết, hãy xem [theo cách thủ công yêu cầu thu thập dữ liệu và lập chỉ mục lại của một trang web, một thư viện hay một danh sách](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Đợi ít nhất 24 giờ sau khi theo cách thủ công yêu cầu một thu thập thông tin và đầy đủ tái lập chỉ mục để xem nếu bạn vẫn gặp sự cố. 

    Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn bắt đầu thu thập dữ liệu và lập chỉ mục lại đầy đủ, xin vui lòng đăng nhập một trường hợp hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.

> [!IMPORTANT]
> Nếu một trang web, tài liệu (thư viện), hoặc một danh sách đã bị xoá và vẫn cho thấy trong kết quả tìm kiếm, người dùng sẽ nhận được một **Lỗi 404 Không tìm thấy tệp** khi cố gắng để truy cập vào nó. Vấn đề này nên được đăng nhập như là một trường hợp hỗ trợ cho điều tra thêm. 



