---
title: Trang web hiện đại như là trang web gốc
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054724"
---
# <a name="modern-site-as-root-site"></a>Trang web hiện đại như trang web gốc

Chúng tôi đã bắt đầu triển khai một tính năng mới mà sẽ cho phép bạn hoán đổi trang web gốc trang web [cổ điển của bạn với một trang web hiện đại](https://docs.microsoft.com/sharepoint/modern-root-site). Sử dụng [gọi SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để hoán đổi vị trí của một trang web với một trang web trong khi lưu trữ các trang web ban đầu. Có sẵn cho cả hai trang web nhóm (không được kết nối với một nhóm) và trang web truyền thông.

>[!Important]
> Không xóa trang web gốc cổ điển của bạn để tạo ra một trang web truyền thông hiện đại. Điều này không được hỗ trợ bởi Microsoft. Xóa các trang web gốc sẽ làm cho tất cả các trang web SharePoint trong tổ chức của bạn không thể truy nhập cho tất cả người dùng, cho đến khi bạn khôi phục lại các trang web hoặc tạo ra một trang web mới tại cùng một URL. Chúng tôi sẽ giao tiếp tính năng này thông qua Trung tâm tin nhắn. Bạn nên mong đợi tính năng được bật trong thuê của bạn ngay.

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề với trao đổi trang web
- Trang đích có thể trả về lỗi "không tìm thấy" (HTTP 404) trong một khoảng thời gian ngắn.
- Nội dung cần phải được thu thập lại để cập nhật chỉ mục tìm kiếm. Không có hướng dẫn sử dụng bước cần thiết ở đây, điều này sẽ được thực hiện tự động.
- Bất cứ điều gì phụ thuộc vào "tĩnh" liên kết (chẳng hạn như tập tin Sync và OneNote tập tin) sẽ cần phải được sửa chữa thủ công.
- Trang web máy chủ dự án có thể cần phải được xác nhận để đảm bảo rằng chúng vẫn được liên kết chính xác. 
