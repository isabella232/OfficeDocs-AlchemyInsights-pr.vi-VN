---
title: Khắc phục sự cố với ghi các thiết bị iOS trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736180"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="42923-102">Khắc phục sự cố với ghi các thiết bị iOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="42923-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="42923-103">Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="42923-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="42923-104">Một số thông báo lỗi phổ biến và giải pháp bước:</span><span class="sxs-lookup"><span data-stu-id="42923-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="42923-105">**Thiết bị Cap đạt** Người dùng có nhiều thiết bị đăng ký hơn giới hạn thiết bị.</span><span class="sxs-lookup"><span data-stu-id="42923-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="42923-106">Hãy đánh giá các tài liệu này để [xóa thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="42923-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="42923-107">**Dịch vụ này không được hỗ trợ. Không có chính sách đăng ký:** dịch vụ thông báo đẩy của Apple (APNS) cần phải được cấu hình hoặc gia hạn.</span><span class="sxs-lookup"><span data-stu-id="42923-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="42923-108">Đánh giá [tài liệu này](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) để biết hướng dẫn về cách thực hiện điều đó.</span><span class="sxs-lookup"><span data-stu-id="42923-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="42923-109">**Người dùng loại giấy phép không hợp lệ hoặc tên người dùng không được công nhận:** Người dùng cần được gán giấy phép InTune hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="42923-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="42923-110">Đánh giá các tài liệu này để gán giấy phép thông qua: [Trung tâm quản trị văn phòng](https://docs.microsoft.com/intune/licenses-assign) hoặc [cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="42923-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="42923-111">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="42923-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="42923-112">Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung.</span><span class="sxs-lookup"><span data-stu-id="42923-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="42923-113">Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="42923-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="42923-114">Đánh giá các tài liệu này để biết danh sách các lỗi phổ biến ngăn đăng ký và giải pháp cho từng: [hướng dẫn khắc phục sự cố](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) và [gỡ rối doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="42923-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="42923-115">[Tìm hiểu cách đăng ký thiết bị iOS trong Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="42923-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

