---
title: nâng cấp lên 932
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806061"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ada70-102">Nâng cấp kết nối Azure AD</span><span class="sxs-lookup"><span data-stu-id="ada70-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ada70-103">Theo mặc định, nâng cấp tự động được bật cho Azure AD Connect, vốn sẽ giúp đảm bảo bạn đang chạy phiên bản mới nhất.</span><span class="sxs-lookup"><span data-stu-id="ada70-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ada70-104">Để xác minh cài đặt nâng cấp tự động, hãy sử dụng lệnh ghép ngắn **Get-ADSyncAutoUpgrade** trong Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ada70-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ada70-105">Lệnh ghép ngắn sẽ trả về một trong các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="ada70-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="ada70-106">Đã **bật**: nâng cấp tự động được bật.</span><span class="sxs-lookup"><span data-stu-id="ada70-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="ada70-107">**Tắt**: nâng cấp tự động bị vô hiệu hóa.</span><span class="sxs-lookup"><span data-stu-id="ada70-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="ada70-108">Bị **tạm ngừng**: Hệ thống không còn đủ điều kiện để nhận các nâng cấp tự động.</span><span class="sxs-lookup"><span data-stu-id="ada70-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ada70-109">Bạn không thể cấu hình giá trị này; nó được đặt bởi hệ thống.</span><span class="sxs-lookup"><span data-stu-id="ada70-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="ada70-110">Để biết thêm thông tin, hãy xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ada70-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="ada70-111">Để tải xuống phiên bản mới nhất của Azure AD Connect, hãy đi tới [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="ada70-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
