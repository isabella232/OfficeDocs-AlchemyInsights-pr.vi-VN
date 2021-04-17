---
title: Thiết bị trình quản lý cấu hình bị thiếu trong cổng thông tin
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817266"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="b7e9c-102">Thiết bị trình quản lý cấu hình bị thiếu trong cổng thông tin</span><span class="sxs-lookup"><span data-stu-id="b7e9c-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="b7e9c-103">Đối với thiết bị đồng bộ để làm việc, các [điểm cuối Internet bắt buộc](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) phải có thể truy nhập được từ máy chủ tại chỗ lưu trữ vai trò điểm kết nối dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="b7e9c-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="b7e9c-104">Để khắc phục sự cố đồng bộ hóa thiết bị, vui lòng xem lại **Cmgatewaysyncuploadworker. log** nằm trên điểm kết nối dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="b7e9c-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="b7e9c-105">Tìm hiểu thêm về đối tượng [thuê đính kèm trong Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="b7e9c-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
