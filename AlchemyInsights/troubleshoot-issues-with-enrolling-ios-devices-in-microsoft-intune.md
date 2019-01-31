---
title: Gỡ rối các vấn đề với đăng ký thiết bị iOS trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658461"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="79a92-102">Gỡ rối các vấn đề với đăng ký thiết bị iOS trong Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="79a92-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="79a92-103">Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.</span><span class="sxs-lookup"><span data-stu-id="79a92-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="79a92-104">Một số thông báo lỗi phổ biến và các bước giải quyết:</span><span class="sxs-lookup"><span data-stu-id="79a92-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="79a92-p101">**Điện thoại nắp đạt** Người dùng có thể thêm các thiết bị ghi danh hơn giới hạn của thiết bị. Xem xét các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="79a92-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="79a92-p102">**Dịch vụ này không được hỗ trợ. Không có chính sách tuyển sinh:** Apple đẩy thông báo dịch vụ (APNS) cần phải được đặt cấu hình hoặc gia hạn. Xem lại [tài liệu này](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) để được hướng dẫn làm thế nào để làm điều đó.</span><span class="sxs-lookup"><span data-stu-id="79a92-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="79a92-p103">**Người dùng giấy phép loại không hợp lệ hoặc không nhận dạng được tên người dùng:** Người dùng cần phải được gán một giấy phép dành hoặc EMS. Xem xét các tài liệu này để gán một giấy phép thông qua: [Trung tâm quản trị văn phòng](https://docs.microsoft.com/intune/licenses-assign) hoặc [cổng Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="79a92-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="79a92-111">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="79a92-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="79a92-p104">Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="79a92-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="79a92-114">Xem xét các tài liệu này cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi: [hướng dẫn giải đáp thắc mắc](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) và [giải đáp thắc mắc doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="79a92-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="79a92-115">[Tìm hiểu làm thế nào để đăng ký thiết bị iOS trong Microsoft dành](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="79a92-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

