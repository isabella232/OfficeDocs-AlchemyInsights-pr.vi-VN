---
title: Khắc phục sự cố với các thiết bị Windows trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665854"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="14749-102">Khắc phục sự cố với các thiết bị Windows trong Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="14749-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="14749-103">Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="14749-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="14749-104">Một số thông báo lỗi phổ biến và giải pháp bước:</span><span class="sxs-lookup"><span data-stu-id="14749-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="14749-105">**Không thể cài đặt phần mềm, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn.</span><span class="sxs-lookup"><span data-stu-id="14749-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="14749-106">Tải lại gói phần mềm máy khách PC trong bảng điều khiển dành cho quản trị viên.</span><span class="sxs-lookup"><span data-stu-id="14749-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="14749-107">Đánh giá tài liệu này để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="14749-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="14749-108">**Mã lỗi 0x801c0003:** Lỗi có thể xảy ra trong các trường hợp sau:</span><span class="sxs-lookup"><span data-stu-id="14749-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="14749-109">Người dùng có nhiều thiết bị đăng ký hơn giới hạn thiết bị.</span><span class="sxs-lookup"><span data-stu-id="14749-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="14749-110">Hãy đánh giá các tài liệu này để [xóa thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="14749-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="14749-111">"Người dùng có thể tham gia thiết bị Azure AD" được đặt thành "không."</span><span class="sxs-lookup"><span data-stu-id="14749-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="14749-112">Đặt nó cho tất cả hoặc chọn người dùng.</span><span class="sxs-lookup"><span data-stu-id="14749-112">Set it to all or select users.</span></span> <span data-ttu-id="14749-113">Đánh giá [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="14749-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="14749-114">Thiết bị đã được đăng ký bởi người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="14749-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="14749-115">Nếu đó là trường hợp, hãy loại bỏ thiết bị khỏi bảng điều khiển Azure InTune hoặc tự hủy đăng ký thiết bị trước khi thử lại.</span><span class="sxs-lookup"><span data-stu-id="14749-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="14749-116">Thiết bị là Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="14749-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="14749-117">Chỉ Windows 10 Pro, Education và Enterprise SKUs có thể tham gia Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14749-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="14749-118">Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:</span><span class="sxs-lookup"><span data-stu-id="14749-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="14749-119">Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung.</span><span class="sxs-lookup"><span data-stu-id="14749-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="14749-120">Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="14749-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="14749-121">Đánh giá các tài liệu này để biết danh sách các lỗi phổ biến ngăn đăng ký và giải pháp cho từng: [hướng dẫn khắc phục sự cố](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) và [gỡ rối doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="14749-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="14749-122">[Tìm hiểu cách đăng ký thiết bị Windows trong Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="14749-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
