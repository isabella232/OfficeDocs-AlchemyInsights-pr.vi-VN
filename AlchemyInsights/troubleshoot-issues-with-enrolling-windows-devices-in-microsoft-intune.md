---
title: Khắc phục sự cố với các thiết bị đăng ký Windows trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808993"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a0211-102">Khắc phục sự cố với các thiết bị đăng ký Windows trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="a0211-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a0211-103">Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="a0211-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a0211-104">Một số thông báo lỗi và giải pháp thông thường:</span><span class="sxs-lookup"><span data-stu-id="a0211-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a0211-105">**Không thể cài đặt phần mềm, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn.</span><span class="sxs-lookup"><span data-stu-id="a0211-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a0211-106">Tải lại gói phần mềm máy khách PC trong bảng điều khiển quản trị InTune.</span><span class="sxs-lookup"><span data-stu-id="a0211-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a0211-107">Xem lại tài liệu này để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="a0211-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a0211-108">**Mã lỗi 0x801c0003:** Lỗi có thể xảy ra trong các tình huống sau đây:</span><span class="sxs-lookup"><span data-stu-id="a0211-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="a0211-109">Người dùng có thêm các thiết bị được đăng ký với giới hạn của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="a0211-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a0211-110">Xem lại các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a0211-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="a0211-111">"Người dùng có thể gia nhập các thiết bị cho Azure AD" được đặt là "không".</span><span class="sxs-lookup"><span data-stu-id="a0211-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="a0211-112">Đặt nó cho tất cả hoặc chọn người dùng.</span><span class="sxs-lookup"><span data-stu-id="a0211-112">Set it to all or select users.</span></span> <span data-ttu-id="a0211-113">Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="a0211-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="a0211-114">Thiết bị này đã được người dùng khác đăng ký.</span><span class="sxs-lookup"><span data-stu-id="a0211-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a0211-115">Nếu trường hợp đó, hãy loại bỏ thiết bị khỏi bàn điều khiển Azure InTune hoặc bỏ đăng ký theo cách thủ công thiết bị trước khi thử lại.</span><span class="sxs-lookup"><span data-stu-id="a0211-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="a0211-116">Thiết bị là Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="a0211-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a0211-117">Chỉ Windows 10 Pro, Education và Enterprise SKUs có thể gia nhập Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a0211-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a0211-118">Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:</span><span class="sxs-lookup"><span data-stu-id="a0211-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="a0211-119">Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp.</span><span class="sxs-lookup"><span data-stu-id="a0211-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a0211-120">Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="a0211-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="a0211-121">Xem lại các tài liệu này để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng: [hướng dẫn khắc phục](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) sự cố và trình [xử lý khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a0211-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a0211-122">[Tìm hiểu cách đăng ký thiết bị Windows trong Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="a0211-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
