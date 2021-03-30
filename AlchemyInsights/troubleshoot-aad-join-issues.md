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
# <a name="troubleshoot-azure-ad-join-issues"></a>Khắc phục sự cố về Azure AD join

1. Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo rằng bạn đã xem xét việc [giới thiệu về quản lý thiết bị trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) sẽ hướng dẫn bạn về cách tải các thiết bị dưới điều khiển để Azure AD. 
1. Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và ghi lại chúng vào InTune, bạn sẽ cần phải đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) tại chỗ trước tiên.
1. Đảm bảo bạn được phép thực hiện các hoạt động trong Azure AD. Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị.
1. Để thực hiện Azure AD join, hãy xem [lập kế hoạch AZURE AD join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Để biết thêm chi tiết về việc giải quyết các sự cố phổ biến với Azure AD join hãy xem [Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) và cho thiết bị chạy Windows 10 Pro, hãy xem [không thể gia nhập Windows 10 Pro MACHINE to Azure AD-need to Upgrade to-Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
