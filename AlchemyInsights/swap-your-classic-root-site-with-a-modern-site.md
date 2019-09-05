---
title: Hoán đổi trang web gốc cổ điển của bạn với một trang web hiện đại
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749282"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Hoán đổi trang web gốc cổ điển của bạn với một trang web hiện đại

Nếu môi trường của bạn đã được thiết lập trước ngày 2019, bạn có thể thay đổi trang web gốc của bạn sang một trang web hiện đại bằng cách sử dụng Microsoft PowerShell:

- Nếu bạn có một trang web khác mà bạn muốn sử dụng làm trang web gốc của bạn, bạn có thể thay thế [(Swap) các trang web gốc](https://docs.microsoft.com/sharepoint/modern-root-site) với nó. 
    - Sử dụng [gọi SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web trong khi lưu trữ các trang web ban đầu. Có sẵn cho cả hai trang web nhóm (không được kết nối với một nhóm) và trang web truyền thông. 

- Khả năng bổ sung sẽ được giới thiệu sớm mà sẽ cho phép bạn tiếp tục sử dụng các nội dung trên trang web, nhưng chuyển đổi các trang web hiện có đến một trang web liên lạc. 
>[!Important]
>Những khả năng này sẽ được cuộn dần. Tiếp tục kiểm tra Office 365 Message Center để cập nhật. 

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề với trao đổi trang web

- Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Nội dung cần phải được thu thập lại để cập nhật chỉ mục tìm kiếm. Không có hướng dẫn sử dụng bước cần thiết-điều này sẽ được thực hiện tự động.
- Bất cứ điều gì phụ thuộc vào "tĩnh" liên kết (chẳng hạn như tập tin Sync và OneNote tập tin) sẽ cần phải được sửa chữa thủ công.
- Nếu trang web nguồn là một trang web tin tức tổ chức, Cập Nhật URL.Nhận danh sách tất cả các trang web tin tức tổ chức.
- Trang web máy chủ dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết chính xác.





