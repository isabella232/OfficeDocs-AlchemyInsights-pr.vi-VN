---
title: Bản ghi thiết bị trùng lặp trong cổng thông tin
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
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790179"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="3f068-102">Bản ghi thiết bị trùng lặp trong cổng thông tin</span><span class="sxs-lookup"><span data-stu-id="3f068-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="3f068-103">Bạn có thể thấy 2 hồ sơ cho một thiết bị trong cổng nếu thiết bị không đúng cách báo cáo trạng thái đồng quản lý trang web quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="3f068-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="3f068-104">Để kiểm tra tình trạng đồng quản lý của thiết bị, xem cột **đồng quản lý** thiết bị trong bảng điều khiển quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="3f068-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="3f068-105">Nếu cột không hiển thị, bạn có thể thêm nó bằng cách bấm chuột phải vào bất kỳ tiêu đề cột nào và chọn nó từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="3f068-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="3f068-106">Giá trị đồng quản lý phải **có**.</span><span class="sxs-lookup"><span data-stu-id="3f068-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="3f068-107">Nếu giá trị là **không**, mở cấu hình quản lý khách hàng applet trên thiết bị khách hàng và kiểm tra thuộc tính **đồng quản lý** trong tab chung.</span><span class="sxs-lookup"><span data-stu-id="3f068-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="3f068-108">Nếu giá trị được **kích hoạt**, điều này cho biết vấn đề với giao tiếp khách hàng quản lý điểm.</span><span class="sxs-lookup"><span data-stu-id="3f068-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="3f068-109">Vui lòng đánh giá **Ccmmessaging. log** trên thiết bị để điều tra vấn đề kết nối tiềm năng.</span><span class="sxs-lookup"><span data-stu-id="3f068-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="3f068-110">Nếu giá trị bị **vô hiệu hoá** và thiết bị được đăng ký trong InTune, hãy đảm bảo rằng thiết bị đã nhận được chính sách đồng quản lý bằng cách xem **Comanagementhandler. log** trên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="3f068-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
