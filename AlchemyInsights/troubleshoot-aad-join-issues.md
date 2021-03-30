---
title: Khắc phục sự cố về Azure AD join
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405766"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="8a3c2-102">Khắc phục sự cố về Azure AD join</span><span class="sxs-lookup"><span data-stu-id="8a3c2-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="8a3c2-103">Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo rằng bạn đã xem xét việc [giới thiệu về quản lý thiết bị trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) sẽ hướng dẫn bạn về cách tải các thiết bị dưới điều khiển để Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a3c2-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="8a3c2-104">Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và ghi lại chúng vào InTune, bạn sẽ cần phải đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) tại chỗ trước tiên.</span><span class="sxs-lookup"><span data-stu-id="8a3c2-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="8a3c2-105">Đảm bảo bạn được phép thực hiện các hoạt động trong Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a3c2-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="8a3c2-106">Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="8a3c2-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="8a3c2-107">Để thực hiện Azure AD join, hãy xem [lập kế hoạch AZURE AD join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="8a3c2-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="8a3c2-108">Để biết thêm chi tiết về việc giải quyết các sự cố phổ biến với Azure AD join hãy xem [Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) và cho thiết bị chạy Windows 10 Pro, hãy xem [không thể gia nhập Windows 10 Pro MACHINE to Azure AD-need to Upgrade to-Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="8a3c2-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
