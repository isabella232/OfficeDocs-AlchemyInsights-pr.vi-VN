---
title: Azure Active Directory join
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405667"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="3b173-102">Azure Active Directory join</span><span class="sxs-lookup"><span data-stu-id="3b173-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="3b173-103">Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo rằng bạn đã xem xét việc [giới thiệu về quản lý thiết bị trong Azure Active Directory](/azure/active-directory/devices/overview) sẽ hướng dẫn bạn về cách tải các thiết bị dưới điều khiển để Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b173-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="3b173-104">Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và ghi lại chúng vào InTune, bạn sẽ cần phải đảm bảo rằng bạn đã [cấu hình InTune](/mem/intune/enrollment/device-enrollment) và có [cấp phép](/mem/intune/fundamentals/licenses-assign) tại chỗ trước tiên.</span><span class="sxs-lookup"><span data-stu-id="3b173-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="3b173-105">Đảm bảo bạn được phép thực hiện các hoạt động trong Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b173-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="3b173-106">Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="3b173-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="3b173-107">Để thực hiện Azure AD join, hãy xem [lập kế hoạch AZURE AD join](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="3b173-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="3b173-108">Để biết thêm chi tiết về việc giải quyết các sự cố phổ biến với Azure AD join, hãy xem [câu hỏi thường gặp về Azure AD join](/azure/active-directory/devices/faq) và cho thiết bị Windows 10 Pro, hãy xem [không thể gia nhập Windows 10 Pro MACHINE to Azure AD-cần nâng cấp lên cộng đồng Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span><span class="sxs-lookup"><span data-stu-id="3b173-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
