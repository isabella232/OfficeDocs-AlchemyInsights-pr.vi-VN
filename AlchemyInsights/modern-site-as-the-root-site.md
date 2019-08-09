---
title: Các trang web hiện đại như các trang web gốc
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269398"
---
# <a name="modern-site-as-root-site"></a>Các trang web hiện đại như là trang web gốc

Chúng tôi đã bắt đầu buổi giới thiệu một tính năng mới mà sẽ cho phép bạn để hoán đổi cổ điển trang web trang web gốc của bạn với một trang web hiện đại. Sử dụng [Gọi SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) để trao đổi vị trí của một trang web với một trang web khác trong khi lưu trữ trang web gốc. Sẵn sàng cho cả hai nhóm trang web (không kết nối với một nhóm) và trang web thông tin liên lạc. 

>[!Important]
> Không xóa bỏ các trang web gốc cổ điển của bạn để tạo ra một trang web thông tin liên lạc hiện đại. Điều này không được hỗ trợ bởi Microsoft. Xóa trang web gốc sẽ làm cho tất cả các trang web SharePoint trong tổ chức của bạn không thể tiếp cận tất cả người dùng, cho đến khi bạn khôi phục lại các trang web hoặc tạo một trang web mới tại cùng một URL. Chúng tôi sẽ liên lạc các tính năng này thông qua Trung tâm tin nhắn. Bạn có thể mong đợi các tính năng được bật trong người thuê nhà của bạn ngay.

## <a name="known-issues-with-swapping-sites"></a>Các vấn đề được biết đến với các trang web trao đổi
- Trang web mục tiêu có thể trả lại một lỗi "không tìm thấy" (HTTP 404) cho một khoảng thời gian ngắn.
- Nội dung sẽ cần phải được recrawled để cập nhật danh mục tìm kiếm. Không không có bước hướng dẫn sử dụng yêu cầu ở đây, điều này sẽ được thực hiện tự động.
- Bất cứ điều gì phụ thuộc vào các liên kết "tĩnh" (chẳng hạn như đồng bộ hóa tập tin và OneNote files) sẽ cần phải được sửa chữa bằng tay.
- Dự án máy chủ trang web có thể cần phải được xác nhận để đảm bảo rằng họ vẫn còn liên kết một cách chính xác. 
