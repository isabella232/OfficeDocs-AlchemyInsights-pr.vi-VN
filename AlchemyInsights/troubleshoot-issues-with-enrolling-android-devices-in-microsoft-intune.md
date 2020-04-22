---
title: Khắc phục sự cố với ghi danh thiết bị Android trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759642"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="30e99-102">Khắc phục sự cố với ghi danh thiết bị Android trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="30e99-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="30e99-103">Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="30e99-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="30e99-104">Một số vấn đề thường gặp và các bước giải quyết:</span><span class="sxs-lookup"><span data-stu-id="30e99-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="30e99-105">**Thiết bị không được mã hoá lỗi trong cổng công ty:** Các phiên bản Android mới hơn, đặc biệt bắt đầu với v 7.0, yêu cầu mật mã khởi động để đảm bảo rằng thiết bị của bạn được mã hóa hoàn toàn.</span><span class="sxs-lookup"><span data-stu-id="30e99-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="30e99-106">Các giải pháp phổ biến là kích hoạt pin khởi động hoặc mã hóa đầy đủ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="30e99-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="30e99-107">Đánh giá [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="30e99-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="30e99-108">**Thiết bị không thể kiểm tra với dịch vụ InTune hoặc hiển thị là "không lành mạnh" trong bảng điều khiển quản trị InTune:** Một số thiết bị Samsung 4,4 và 5,5 có thể không kiểm tra vào dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="30e99-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="30e99-109">Có 3 giải pháp có thể cho vấn đề này:</span><span class="sxs-lookup"><span data-stu-id="30e99-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="30e99-110">Mở thủ công ứng dụng cổng thông tin công ty InTune, sẽ tự động khởi tạo đồng bộ hóa thiết bị.</span><span class="sxs-lookup"><span data-stu-id="30e99-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="30e99-111">Cập Nhật thiết bị lên Android 6,0 trở lên.</span><span class="sxs-lookup"><span data-stu-id="30e99-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="30e99-112">Vô hiệu hoá Samsung Smart Manager từ quản lý cổng thông tin công ty InTune.</span><span class="sxs-lookup"><span data-stu-id="30e99-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="30e99-113">Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) để biết thêm chi tiết về các vấn đề và nghị quyết.</span><span class="sxs-lookup"><span data-stu-id="30e99-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="30e99-114">**Người dùng loại giấy phép không hợp lệ** hoặc **tên người dùng không được nhận dạng lỗi:** người dùng cần được gán một giấy phép InTune hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="30e99-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="30e99-115">Đánh giá các tài liệu này để gán giấy phép thông qua: Trung tâm quản trị văn phòng hoặc cổng thông tin Azure.</span><span class="sxs-lookup"><span data-stu-id="30e99-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="30e99-116">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="30e99-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="30e99-117">Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung.</span><span class="sxs-lookup"><span data-stu-id="30e99-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="30e99-118">Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="30e99-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="30e99-119">Đánh giá [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) để biết danh sách các lỗi phổ biến ngăn chặn đăng ký và giải pháp cho mỗi.</span><span class="sxs-lookup"><span data-stu-id="30e99-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="30e99-120">[Tìm hiểu cách đăng ký thiết bị Android trong Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="30e99-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
