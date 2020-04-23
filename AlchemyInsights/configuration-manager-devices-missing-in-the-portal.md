---
title: Quản lý cấu hình thiết bị thiếu trong cổng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790239"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="f91f4-102">Quản lý cấu hình thiết bị thiếu trong cổng</span><span class="sxs-lookup"><span data-stu-id="f91f4-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="f91f4-103">Để thiết bị đồng bộ hoá hoạt động, điểm [cuối Internet bắt buộc](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) phải có thể truy cập từ máy chủ tại nơi lưu trữ vai trò kết nối dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="f91f4-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="f91f4-104">Để khắc phục sự cố đồng bộ hoá thiết bị, vui lòng đánh giá **Cmgatewaysyncuploadworker. log** nằm trên điểm kết nối dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="f91f4-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="f91f4-105">Tìm hiểu thêm về [người thuê đính kèm trong Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="f91f4-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
