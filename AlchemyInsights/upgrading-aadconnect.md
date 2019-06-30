---
title: 932 nâng cấp AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365939"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="8aa0b-102">Nâng cấp Azure quảng cáo kết nối</span><span class="sxs-lookup"><span data-stu-id="8aa0b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="8aa0b-103">Theo mặc định, nâng cấp tự động được kích hoạt cho Azure quảng cáo kết nối, giúp đảm bảo rằng bạn đang chạy phiên bản mới nhất.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="8aa0b-104">Để xác minh các cài đặt nâng cấp tự động, sử dụng lệnh ghép ngắn **Get-ADSyncAutoUpgrade** Azure quảng cáo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="8aa0b-105">Lệnh ghép ngắn sẽ trả về một giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="8aa0b-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="8aa0b-106">**Enabled**: nâng cấp tự động được kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="8aa0b-107">**Vô hiệu hóa**: nâng cấp tự động bị vô hiệu hóa.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="8aa0b-108">**Bị treo**: Hệ thống không còn đủ điều kiện để nhận được tự động nâng cấp.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="8aa0b-109">Bạn không thể đặt cấu hình các giá trị này; khách sạn nằm trong hệ thống.</span><span class="sxs-lookup"><span data-stu-id="8aa0b-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="8aa0b-110">Để biết thêm thông tin, hãy xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="8aa0b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="8aa0b-111">Để tải xuống phiên bản mới nhất của Azure quảng cáo kết nối, đi đến [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="8aa0b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
