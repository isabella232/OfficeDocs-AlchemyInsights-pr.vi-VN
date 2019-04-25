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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390665"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="602a4-102">Gỡ rối các vấn đề với đăng ký thiết bị Windows trong Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="602a4-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="602a4-103">Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.</span><span class="sxs-lookup"><span data-stu-id="602a4-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="602a4-104">Một số thông báo lỗi phổ biến và các bước giải quyết:</span><span class="sxs-lookup"><span data-stu-id="602a4-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="602a4-105">**Phần mềm không cần cài đặt, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn.</span><span class="sxs-lookup"><span data-stu-id="602a4-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="602a4-106">Tái tải về gói phần mềm máy tính khách hàng trong giao diện điều khiển Admin dành.</span><span class="sxs-lookup"><span data-stu-id="602a4-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="602a4-107">Xem lại tài liệu này cho biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="602a4-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="602a4-108">**Mã lỗi 0x801c0003:** Các lỗi có thể xảy ra trong các trường hợp sau:</span><span class="sxs-lookup"><span data-stu-id="602a4-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="602a4-109">Người dùng có thể thêm các thiết bị ghi danh hơn giới hạn của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="602a4-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="602a4-110">Xem xét các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="602a4-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="602a4-111">"Người dùng có thể tham gia vào thiết bị để Azure quảng cáo" được thiết lập để "không".</span><span class="sxs-lookup"><span data-stu-id="602a4-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="602a4-112">Thiết lập nó cho tất cả hoặc chọn người dùng.</span><span class="sxs-lookup"><span data-stu-id="602a4-112">Set it to all or select users.</span></span> <span data-ttu-id="602a4-113">Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="602a4-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="602a4-114">Thiết bị đã được đăng ký bởi người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="602a4-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="602a4-115">Nếu trường hợp đó xảy ra, loại bỏ các thiết bị từ bàn điều khiển Azure dành hoặc tự unenroll thiết bị trước khi thử lại.</span><span class="sxs-lookup"><span data-stu-id="602a4-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="602a4-116">Thiết là Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="602a4-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="602a4-117">Chỉ Windows 10 Pro, giáo dục và doanh nghiệp SKUs có thể tham gia vào Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="602a4-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="602a4-118">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="602a4-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="602a4-119">Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại.</span><span class="sxs-lookup"><span data-stu-id="602a4-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="602a4-120">Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="602a4-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="602a4-121">Xem xét các tài liệu này cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi: [hướng dẫn giải đáp thắc mắc](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) và [giải đáp thắc mắc doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="602a4-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="602a4-122">[Tìm hiểu làm thế nào để đăng ký thiết bị Windows trong Microsoft dành](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="602a4-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

