---
title: Khắc phục sự cố với các thiết bị đăng ký iOS trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669270"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="3a755-102">Khắc phục sự cố với các thiết bị đăng ký iOS trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="3a755-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="3a755-103">Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="3a755-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="3a755-104">Một số thông báo lỗi và giải pháp thông thường:</span><span class="sxs-lookup"><span data-stu-id="3a755-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="3a755-105">**Nắp thiết bị đã đạt** Người dùng có thêm các thiết bị được đăng ký với giới hạn của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="3a755-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3a755-106">Xem lại các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3a755-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="3a755-107">**Dịch vụ này không được hỗ trợ. Không có chính sách đăng ký:** dịch vụ thông báo đẩy táo (APNS) cần được cấu hình hoặc gia hạn.</span><span class="sxs-lookup"><span data-stu-id="3a755-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="3a755-108">Xem lại [tài liệu này](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) để biết hướng dẫn về cách thực hiện điều đó.</span><span class="sxs-lookup"><span data-stu-id="3a755-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="3a755-109">**Loại giấy phép người dùng không được nhận diện không hợp lệ hoặc tên người dùng:** Người dùng cần được gán giấy phép InTune hoặc EMS.</span><span class="sxs-lookup"><span data-stu-id="3a755-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3a755-110">Xem lại các tài liệu này để gán giấy phép thông qua: [Trung tâm quản trị Office](https://docs.microsoft.com/intune/licenses-assign) hoặc [cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="3a755-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="3a755-111">Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:</span><span class="sxs-lookup"><span data-stu-id="3a755-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3a755-112">Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp.</span><span class="sxs-lookup"><span data-stu-id="3a755-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3a755-113">Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="3a755-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="3a755-114">Xem lại các tài liệu này để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng: [hướng dẫn khắc phục](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) sự cố và trình [xử lý khắc phục sự cố](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3a755-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="3a755-115">[Tìm hiểu cách đăng ký thiết bị iOS trong Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="3a755-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

