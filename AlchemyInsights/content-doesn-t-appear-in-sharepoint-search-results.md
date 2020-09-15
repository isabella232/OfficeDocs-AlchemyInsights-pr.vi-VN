---
title: Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713152"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint

Hãy làm theo các bước khắc phục sự cố này khi nội dung được dự kiến không xuất hiện trong kết quả tìm kiếm:
  
1. Kiểm tra xem **trang** có chứa nội dung được dự kiến được đặt là cho phép nội dung xuất hiện trong kết quả tìm kiếm hay không. Làm theo các bước trong [Hiển thị nội dung trên một trang trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kiểm tra xem **danh sách** hoặc **Thư viện** có chứa nội dung được dự kiến được đặt là cho phép nội dung xuất hiện trong kết quả tìm kiếm hay không. Làm theo các bước trong [Hiển thị nội dung từ danh sách hoặc thư viện trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Xác minh rằng trang, tài liệu hoặc bố trí trang tùy chỉnh được phát hành dưới dạng **Phiên bản chính.** Làm theo bước 3 trong [Tìm kiếm không trả về tất cả các kết quả trong SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Xác nhận rằng người dùng có **quyền** xem nội dung. Làm theo các bước trong [Tìm hiểu các mức cấp phép trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Nếu sơ đồ tìm kiếm đã được thay đổi bằng cách thêm một thuộc tính được quản lý mới, bằng cách sửa thuộc tính được quản lý hoặc loại bỏ một thuộc tính được quản lý sau đó yêu cầu thu thập và chỉ mục lại sẽ được yêu cầu. Lập **chỉ mục lại** nội dung bằng cách thực hiện theo các bước bằng cách thủ công theo [yêu cầu thu thập và lập chỉ mục lại một site, một thư viện hoặc danh sách](https://docs.microsoft.com/sharepoint/crawl-site-content). Việc này có thể mất một lúc, chờ 24 giờ trước khi kiểm tra lại kết quả.

Để biết thêm thông tin, hãy xem mục [bật nội dung trên một trang để có thể tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
