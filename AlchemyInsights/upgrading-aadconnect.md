---
title: 932 nâng cấp AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778763"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ac3f4-102">Nâng cấp Azure quảng cáo kết nối</span><span class="sxs-lookup"><span data-stu-id="ac3f4-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ac3f4-103">Theo mặc định, nâng cấp tự động được kích hoạt cho Azure quảng cáo kết nối, giúp đảm bảo rằng bạn đang chạy phiên bản mới nhất.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ac3f4-104">Để xác minh các cài đặt nâng cấp tự động, sử dụng lệnh ghép ngắn **Get-ADSyncAutoUpgrade** Azure quảng cáo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ac3f4-105">Lệnh ghép ngắn sẽ trả về một giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="ac3f4-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="ac3f4-106">**Enabled**: nâng cấp tự động được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="ac3f4-107">**Vô hiệu hóa**: nâng cấp tự động bị vô hiệu hóa.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="ac3f4-108">**Bị treo**: Hệ thống không còn đủ điều kiện để nhận được tự động nâng cấp.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ac3f4-109">Bạn không thể đặt cấu hình các giá trị này; khách sạn nằm trong hệ thống.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="ac3f4-110">Để biết thêm thông tin, hãy xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="ac3f4-111">Để tải xuống phiên bản mới nhất của Azure quảng cáo kết nối, đi đến [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

