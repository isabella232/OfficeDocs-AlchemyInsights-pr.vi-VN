---
title: Chẩn đoán cho các sự cố truy nhập cổng khác nhau
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030924"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Chẩn đoán cho các sự cố truy nhập cổng khác nhau

Để giải quyết các vấn đề truy nhập cổng khác nhau, hãy thực hiện các bước sau đây:

1. Dừng/giải quyết máy ảo (VM) khỏi cổng thông tin, khởi động lại máy ảo và thử lại. 
2. Kiểm tra cài đặt mạng cho máy ảo của bạn để xác định xem liệu bạn có chặn lưu lượng truy cập cho Nhóm Bảo mật Mạng (NSG) không. Bạn cũng có thể sử dụng công cụ xác minh dòng [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) của Bộ theo dõi Mạng để kiểm tra các NSG đang chặn lưu lượng, Tuyến đường User-Defined (UDR) đang định tuyến lưu lượng trở lại tại chỗ ('Tuyến đường Mặc định' 0.0.0.0/0) hoặc về thiết bị mạng.
Nếu bạn vẫn gặp phải sự cố sau khi thử các bước ở trên, vui lòng cung cấp tên VM và cổng TCP mà bạn đang cố gắng gửi thư để chẩn đoán thêm.

**Tài liệu được Đề xuất**

[Các giới hạn và đề xuất về việc gửi email đi qua cổng 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)