---
title: Chẩn đoán các sự cố truy nhập cổng khác nhau
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036803"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Chẩn đoán các sự cố truy nhập cổng khác nhau

Để giải quyết các vấn đề truy nhập khác nhau của cổng, hãy thực hiện các bước sau đây:

1. Dừng/hủy phân bổ máy ảo (VM) từ cổng thông tin, khởi động lại VM và thử lại. 
2. Kiểm tra thiết đặt mạng của VM của bạn để xác định xem bạn có lưu lượng truy nhập nhóm bảo mật mạng (NSGs) không. Bạn cũng có thể sử dụng [công cụ xác minh dòng IP của Watcher của Network](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) để kiểm tra việc chặn lưu lượng truy cập nsgs, các tuyến đường User-Defined (udrs) sẽ truy cập vào giao thông của bạn trở lại thiết bị tại cơ sở (' định tuyến 0.0.0.0/0) hoặc đến một thiết bị mạng.
Nếu bạn vẫn gặp sự cố sau khi thử các bước ở trên, vui lòng cung cấp tên VM và cổng TCP mà bạn đang cố gắng gửi thư để biết thêm về chẩn đoán.

**Tài liệu được đề xuất**

[Các giới hạn và đề xuất để gửi email đi qua cổng 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)