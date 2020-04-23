---
title: 932 nâng cấp AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766515"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f3aa4-102">Nâng cấp Azure AD kết nối</span><span class="sxs-lookup"><span data-stu-id="f3aa4-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f3aa4-103">Theo mặc định, tính năng nâng cấp tự động được bật cho Azure AD Connect, giúp đảm bảo bạn đang chạy phiên bản mới nhất.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f3aa4-104">Để xác minh cài đặt tự động nâng cấp, sử dụng lệnh **Get-ADSyncAutoUpgrade** Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f3aa4-105">Lệnh này sẽ trả về một trong các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="f3aa4-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f3aa4-106">**Kích hoạt**: tự động nâng cấp được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f3aa4-107">**Vô hiệu hoá**: tự động nâng cấp bị vô hiệu hoá.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f3aa4-108">Bị **tạm ngưng**: Hệ thống không còn đủ điều kiện để nhận các nâng cấp tự động.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f3aa4-109">Bạn không thể cấu hình giá trị này; nó được thiết lập bởi hệ thống.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f3aa4-110">Để biết thêm thông tin, xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="f3aa4-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f3aa4-111">Để tải xuống phiên bản mới nhất của Azure AD kết nối [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594), hãy chuyển đến.</span><span class="sxs-lookup"><span data-stu-id="f3aa4-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
