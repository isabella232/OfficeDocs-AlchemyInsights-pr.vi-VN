---
title: Bản ghi thiết bị trùng lặp trong cổng thông tin
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678526"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="20fdc-102">Bản ghi thiết bị trùng lặp trong cổng thông tin</span><span class="sxs-lookup"><span data-stu-id="20fdc-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="20fdc-103">Bạn có thể thấy 2 bản ghi cho một thiết bị trong cổng thông tin nếu thiết bị không chính xác báo cáo trạng thái quản lý đồng bộ với site trình quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="20fdc-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="20fdc-104">Để kiểm tra trạng thái đồng quản lý của một thiết bị, hãy xem lại cột **đồng quản lý** cho thiết bị trong bảng điều khiển trình quản lý cấu hình.</span><span class="sxs-lookup"><span data-stu-id="20fdc-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="20fdc-105">Nếu cột không hiển thị, bạn có thể thêm nó bằng cách bấm chuột phải vào bất kỳ tiêu đề cột nào, rồi chọn nó từ danh sách.</span><span class="sxs-lookup"><span data-stu-id="20fdc-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="20fdc-106">Giá trị đồng quản lý phải **có**.</span><span class="sxs-lookup"><span data-stu-id="20fdc-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="20fdc-107">Nếu giá trị là **không**, hãy mở applet máy khách trình quản lý cấu hình trên thiết bị khách và kiểm tra thuộc tính **đồng quản lý** trong tab chung.</span><span class="sxs-lookup"><span data-stu-id="20fdc-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="20fdc-108">Nếu giá trị được **bật**, điều này cho biết sự cố với giao tiếp khách hàng với điểm quản lý.</span><span class="sxs-lookup"><span data-stu-id="20fdc-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="20fdc-109">Vui lòng xem **CcmMessaging. log** trên thiết bị để điều tra các vấn đề kết nối tiềm ẩn.</span><span class="sxs-lookup"><span data-stu-id="20fdc-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="20fdc-110">Nếu giá trị bị **vô hiệu hóa** và thiết bị được đăng ký trong InTune, vui lòng đảm bảo rằng thiết bị đã nhận được chính sách đồng quản lý bằng cách xem lại **Comanagementhandler. đăng nhập** vào thiết bị.</span><span class="sxs-lookup"><span data-stu-id="20fdc-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
