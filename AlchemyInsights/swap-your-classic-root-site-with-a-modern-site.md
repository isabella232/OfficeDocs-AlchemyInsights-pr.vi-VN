---
title: Trao đổi trang web gốc cổ điển của bạn với một trang web hiện đại
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270766"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trao đổi trang web gốc cổ điển của bạn với một trang web hiện đại

Nếu môi trường của bạn đã được thiết lập trước khi tháng tư 2019, bạn có thể thay đổi trang web gốc của bạn vào một trang web hiện đại bằng cách sử dụng Microsoft PowerShell:

- Nếu bạn có một trang web khác mà bạn muốn sử dụng như là trang web gốc của bạn, bạn có thể thay thế (trao đổi) gốc trang web với nó. 
    - Sử dụng [Gọi SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để trao đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang web gốc. Sẵn sàng cho cả hai nhóm trang web (không kết nối với một nhóm) và trang web thông tin liên lạc. 

- Bổ sung khả năng sẽ được giới thiệu sớm mà sẽ cho phép bạn tiếp tục sử dụng nội dung trên trang web, nhưng chuyển đổi trang web hiện có để một trang web thông tin liên lạc. 
>[!Important]
>Những khả năng sẽ được cuộn ra dần dần. Tiếp tục để kiểm tra xem Trung tâm thông báo Office 365 bản Cập Nhật. 

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề được biết đến với các trang web trao đổi

- Trang web mục tiêu có thể trả lại một lỗi "không tìm thấy" (HTTP 404) cho một khoảng thời gian ngắn.
- Nội dung sẽ cần phải được recrawled để cập nhật danh mục tìm kiếm. Có không có bước hướng dẫn sử dụng yêu cầu - điều này sẽ được thực hiện tự động.
- Bất cứ điều gì phụ thuộc vào các liên kết "tĩnh" (chẳng hạn như đồng bộ hóa tập tin và OneNote files) sẽ cần phải được sửa chữa bằng tay.
- Nếu trang web mã nguồn là một trang web tổ chức tin tức, Cập Nhật URL.Nhận được một danh sách tất cả các trang web tin tức tổ chức.
- Dự án máy chủ trang web có thể cần phải được xác nhận để đảm bảo rằng họ vẫn còn liên kết một cách chính xác.





