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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="d747f-102">Chẩn đoán các sự cố truy nhập cổng khác nhau</span><span class="sxs-lookup"><span data-stu-id="d747f-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="d747f-103">Để giải quyết các vấn đề truy nhập khác nhau của cổng, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="d747f-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="d747f-104">Dừng/hủy phân bổ máy ảo (VM) từ cổng thông tin, khởi động lại VM và thử lại.</span><span class="sxs-lookup"><span data-stu-id="d747f-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="d747f-105">Kiểm tra thiết đặt mạng của VM của bạn để xác định xem bạn có lưu lượng truy nhập nhóm bảo mật mạng (NSGs) không.</span><span class="sxs-lookup"><span data-stu-id="d747f-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="d747f-106">Bạn cũng có thể sử dụng [công cụ xác minh dòng IP của Watcher của Network](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) để kiểm tra việc chặn lưu lượng truy cập nsgs, các tuyến đường User-Defined (udrs) sẽ truy cập vào giao thông của bạn trở lại thiết bị tại cơ sở (' định tuyến 0.0.0.0/0) hoặc đến một thiết bị mạng.</span><span class="sxs-lookup"><span data-stu-id="d747f-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="d747f-107">Nếu bạn vẫn gặp sự cố sau khi thử các bước ở trên, vui lòng cung cấp tên VM và cổng TCP mà bạn đang cố gắng gửi thư để biết thêm về chẩn đoán.</span><span class="sxs-lookup"><span data-stu-id="d747f-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="d747f-108">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="d747f-108">**Recommended Documents**</span></span>

[<span data-ttu-id="d747f-109">Các giới hạn và đề xuất để gửi email đi qua cổng 25</span><span class="sxs-lookup"><span data-stu-id="d747f-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)