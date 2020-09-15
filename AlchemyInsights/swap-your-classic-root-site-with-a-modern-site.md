---
title: Trao đổi site gốc cổ điển của bạn với site hiện đại
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691201"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trao đổi site gốc cổ điển của bạn với site hiện đại

Nếu môi trường của bạn đã được thiết lập trước ngày 2019 tháng 4, bạn có thể thay đổi site gốc của bạn với một site hiện đại bằng cách sử dụng Microsoft PowerShell:

- Nếu bạn có một trang khác mà bạn muốn dùng làm site gốc của mình, bạn có thể thay thế [(hoán đổi) trang gốc](https://docs.microsoft.com/sharepoint/modern-root-site) với nó. 
    - Sử dụng cuộc [gọi-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang gốc. Sẵn dùng cho cả site nhóm (không được kết nối với một nhóm) và site liên lạc. 

- Các chức năng bổ sung sẽ sớm được giới thiệu sẽ cho phép bạn tiếp tục sử dụng nội dung trên trang, nhưng chuyển đổi site hiện có vào một site liên lạc. 
>[!Important]
>Những khả năng này sẽ được thực hiện dần dần. Tiếp tục kiểm tra Trung tâm thông báo cho các bản Cập Nhật. 

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề đã biết với việc trao đổi site

- Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Nội dung sẽ cần được recrawled để cập nhật chỉ mục tìm kiếm. Không có bước thủ công nào cần thiết-điều này sẽ được tự động hoàn tất.
- Bất kỳ điều gì phụ thuộc vào các nối kết "tĩnh" (chẳng hạn như tệp đồng bộ tệp và tệp OneNote) sẽ cần được sửa chữa theo cách thủ công.
- Nếu trang nguồn là một trang tin tức tổ chức, hãy cập nhật URL.Lấy danh sách tất cả các trang tin tức của tổ chức.
- Các trang web dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết đúng.
