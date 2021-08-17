---
title: Nội dung không xuất hiện trong kết quả SharePoint kiếm
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081632"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Nội dung không xuất hiện trong kết quả SharePoint kiếm

Thực hiện theo các bước khắc phục sự cố này khi nội dung dự kiến không xuất hiện trong kết quả tìm kiếm:
  
1. Kiểm tra xem **site có chứa** nội dung dự kiến đã được thiết lập để cho phép nội dung xuất hiện trong kết quả tìm kiếm không. Làm theo các bước trong mục [Hiển thị nội dung trên site trong kết quả tìm kiếm.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Kiểm tra xem danh **sách hay** thư **viện có** chứa nội dung dự kiến đã được thiết lập để cho phép nội dung xuất hiện trong kết quả tìm kiếm hay chưa. Làm theo các bước trong mục [Hiển thị nội dung từ danh sách hoặc thư viện trong kết quả tìm kiếm.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Xác nhận rằng bố trí trang, tài liệu hoặc trang tùy chỉnh được phát hành dưới dạng **phiên bản Chính.** Làm theo bước 3 trong [Tìm kiếm không trả về tất cả kết quả trong SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Xác nhận rằng người dùng có **quyền** xem nội dung. Làm theo các bước trong [Mục Hiểu các mức quyền trong SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required. **Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content). Việc này có thể mất một lúc, hãy chờ 24 giờ trước khi kiểm tra lại kết quả.

Để biết thêm thông tin, [hãy xem mục Bật nội dung trên site để bạn có thể tìm kiếm.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
