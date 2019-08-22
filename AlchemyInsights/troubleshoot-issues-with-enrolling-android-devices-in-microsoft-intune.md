---
title: Gỡ rối các vấn đề với đăng ký các thiết bị Android trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500093"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ccdac-102">Gỡ rối các vấn đề với đăng ký các thiết bị Android trong Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ccdac-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ccdac-103">Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.</span><span class="sxs-lookup"><span data-stu-id="ccdac-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ccdac-104">Một số vấn đề thường gặp và các bước giải quyết:</span><span class="sxs-lookup"><span data-stu-id="ccdac-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ccdac-105">**Thiết bị không mã hóa lỗi vào cổng thông tin công ty:** Các phiên bản mới hơn của Android, đặc biệt là bắt đầu với v7.0, yêu cầu mã khóa khởi động để đảm bảo rằng thiết bị của bạn đã được mã hóa hoàn toàn.</span><span class="sxs-lookup"><span data-stu-id="ccdac-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ccdac-106">Giải pháp phổ biến là để kích hoạt một pin khởi động hoặc đầy đủ mã hóa thiết bị.</span><span class="sxs-lookup"><span data-stu-id="ccdac-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ccdac-107">Xem lại [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) cho biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="ccdac-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ccdac-108">**Thiết bị không kiểm tra tại với các dịch vụ dành hoặc hiển thị là "Không lành mạnh" trong giao diện điều khiển admin dành:** Một số 4,4 Samsung và các thiết bị 5.5 có thể không đánh dấu vào dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="ccdac-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ccdac-109">3 các giải pháp cho vấn đề này có:</span><span class="sxs-lookup"><span data-stu-id="ccdac-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ccdac-110">Tự mở ứng dụng cổng thông tin công ty dành, sẽ tự động bắt đầu một đồng bộ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="ccdac-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ccdac-111">Cập nhật các thiết bị Android 6.0 hoặc cao hơn.</span><span class="sxs-lookup"><span data-stu-id="ccdac-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ccdac-112">Vô hiệu hóa Samsung Smart Manager quản lý cổng thông tin công ty dành.</span><span class="sxs-lookup"><span data-stu-id="ccdac-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ccdac-113">Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) cho biết thêm chi tiết về các vấn đề và độ phân giải.</span><span class="sxs-lookup"><span data-stu-id="ccdac-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ccdac-114">**Không hợp người dùng giấy phép loại lệ** hoặc **dùng tên không công nhận lỗi:** người sử dụng cần phải được gán một giấy phép dành hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="ccdac-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ccdac-115">Xem xét các tài liệu này để gán một giấy phép thông qua: Cổng thông tin Trung tâm quản trị văn phòng hoặc Azure.</span><span class="sxs-lookup"><span data-stu-id="ccdac-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ccdac-116">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="ccdac-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ccdac-117">Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại.</span><span class="sxs-lookup"><span data-stu-id="ccdac-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ccdac-118">Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="ccdac-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ccdac-119">Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi.</span><span class="sxs-lookup"><span data-stu-id="ccdac-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ccdac-120">[Tìm hiểu làm thế nào để đăng ký các thiết bị Android trong Microsoft dành](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ccdac-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
