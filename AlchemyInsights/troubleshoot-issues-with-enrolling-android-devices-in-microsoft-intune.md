---
title: Khắc phục sự cố với các thiết bị Android đăng ký trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689976"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="5d755-102">Khắc phục sự cố với các thiết bị Android đăng ký trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="5d755-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="5d755-103">Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="5d755-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="5d755-104">Một số vấn đề và giải pháp thông thường:</span><span class="sxs-lookup"><span data-stu-id="5d755-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="5d755-105">**Lỗi thiết bị không được mã hóa trong cổng thông tin công ty:** Các phiên bản Android mới hơn, đặc biệt bắt đầu bằng v 7.0, yêu cầu phải có mã khóa khởi động để đảm bảo rằng thiết bị của bạn đã được mã hóa hoàn toàn.</span><span class="sxs-lookup"><span data-stu-id="5d755-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="5d755-106">Các giải pháp phổ biến là bật mã pin khởi động hoặc mã hóa đầy đủ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="5d755-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="5d755-107">Xem lại [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="5d755-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="5d755-108">**Thiết bị không kiểm nhập bằng dịch vụ InTune hoặc hiển thị như "không lành mạnh" trong bảng điều khiển quản trị InTune:** Một số thiết bị Samsung 4,4 và 5,5 có thể không kiểm tra dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="5d755-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="5d755-109">Có 3 giải pháp có thể xảy ra với sự cố này:</span><span class="sxs-lookup"><span data-stu-id="5d755-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="5d755-110">Mở ứng dụng InTune Company Portal theo cách thủ công, điều này sẽ tự động khởi tạo đồng bộ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="5d755-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="5d755-111">Cập Nhật thiết bị lên Android 6,0 trở lên.</span><span class="sxs-lookup"><span data-stu-id="5d755-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="5d755-112">Tắt trình quản lý thông minh Samsung từ quản lý cổng thông tin công ty InTune.</span><span class="sxs-lookup"><span data-stu-id="5d755-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="5d755-113">Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) để biết thêm chi tiết về các sự cố và độ phân giải này.</span><span class="sxs-lookup"><span data-stu-id="5d755-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="5d755-114">Lỗi **người dùng nhập không hợp lệ** hoặc **tên người dùng không được nhận diện:** người dùng cần phải được giao một giấy phép InTune hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="5d755-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="5d755-115">Xem lại các tài liệu này để gán giấy phép thông qua: Trung tâm quản trị Office hoặc cổng thông tin Azure.</span><span class="sxs-lookup"><span data-stu-id="5d755-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="5d755-116">Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:</span><span class="sxs-lookup"><span data-stu-id="5d755-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="5d755-117">Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp.</span><span class="sxs-lookup"><span data-stu-id="5d755-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5d755-118">Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="5d755-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="5d755-119">Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng người.</span><span class="sxs-lookup"><span data-stu-id="5d755-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="5d755-120">[Tìm hiểu cách đăng ký thiết bị Android trong Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="5d755-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
