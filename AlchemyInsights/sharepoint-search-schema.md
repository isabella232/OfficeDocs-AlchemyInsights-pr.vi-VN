---
title: Quản lý lược đồ tìm kiếm trong SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 8eb0e93ea5bbf2154213274041b28a3c908090dae724b8f8e55fa2fb05f16d86
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085106"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>Quản lý lược đồ tìm kiếm trong SharePoint Online

Lược đồ tìm kiếm kiểm soát nội dung mà người dùng có thể tìm kiếm, cách người dùng có thể tìm kiếm và cách bạn có thể trình bày kết quả trên website tìm kiếm của mình. 

Xem [mục Quản lý Lược đồ Tìm kiếm trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) để tìm hiểu cách: 
- Thay đổi lược đồ tìm kiếm.
- Tạo thuộc tính được quản lý.
- Map crawled map crawled properties to managed properties.

Lưu ý những điều sau đây liên quan đến việc quản lý Sơ đồ Tìm kiếm của bạn:

- Nếu bạn nhận được cảnh báo cho **biết** ứng dụng bị tạm dừng khi thực hiện thay đổi sơ đồ thì đây chỉ là tạm thời khi hoạt động bảo trì dịch vụ đang diễn ra. 

    Nếu hơn 24 giờ trôi qua và bạn vẫn gặp phải cảnh báo, vui lòng ghi nhật ký trường hợp hỗ trợ.
- When you change managed properties or add new ones, the changes take only after the content has been re-crawled. In SharePoint Online, crawling happens automatically based on the defined crawl schedule.
- To make sure that your changes are crawled, you can [specifically request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) 

Để có cái nhìn tổng quan đầy đủ về Lược đồ Tìm kiếm, hãy [xem Giới thiệu Sơ đồ Tìm kiếm](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) 


