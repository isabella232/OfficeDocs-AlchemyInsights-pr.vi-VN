---
title: Gỡ rối các vấn đề với đăng ký thiết bị Windows trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934798"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="813cb-102">Gỡ rối các vấn đề với đăng ký thiết bị Windows trong Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="813cb-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="813cb-103">Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.</span><span class="sxs-lookup"><span data-stu-id="813cb-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="813cb-104">Một số thông báo lỗi phổ biến và các bước giải quyết:</span><span class="sxs-lookup"><span data-stu-id="813cb-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="813cb-p101">**Phần mềm không cần cài đặt, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn. Tái tải về gói phần mềm máy tính khách hàng trong giao diện điều khiển Admin dành. Xem lại tài liệu này cho biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="813cb-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="813cb-108">**Mã lỗi 0x801c0003:** Các lỗi có thể xảy ra trong các trường hợp sau:</span><span class="sxs-lookup"><span data-stu-id="813cb-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="813cb-p102">Người dùng có thể thêm các thiết bị ghi danh hơn giới hạn của thiết bị. Xem xét các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="813cb-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="813cb-p103">"Người dùng có thể tham gia vào thiết bị để Azure quảng cáo" được thiết lập để "không". Thiết lập nó cho tất cả hoặc chọn người dùng. Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="813cb-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="813cb-p104">Thiết bị đã được đăng ký bởi người dùng khác. Nếu trường hợp đó xảy ra, loại bỏ các thiết bị từ bàn điều khiển Azure dành hoặc tự unenroll thiết bị trước khi thử lại.</span><span class="sxs-lookup"><span data-stu-id="813cb-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="813cb-p105">Thiết là Windows 10 Home. Chỉ Windows 10 Pro, giáo dục và doanh nghiệp SKUs có thể tham gia vào Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="813cb-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="813cb-118">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="813cb-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="813cb-p106">Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="813cb-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="813cb-121">Xem xét các tài liệu này cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi: [hướng dẫn giải đáp thắc mắc](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) và [giải đáp thắc mắc doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="813cb-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="813cb-122">[Tìm hiểu làm thế nào để đăng ký thiết bị Windows trong Microsoft dành](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="813cb-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

