---
title: Vấn đề về chủ sở hữu đăng ký ứng dụng
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405326"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="c0c7a-102">Vấn đề về chủ sở hữu đăng ký ứng dụng</span><span class="sxs-lookup"><span data-stu-id="c0c7a-102">App Registration Owner issues</span></span>

<span data-ttu-id="c0c7a-103">Sau đây là các phương pháp sẵn dùng để thêm hiệu trưởng với tư cách là chủ sở hữu cho đăng ký ứng dụng:</span><span class="sxs-lookup"><span data-stu-id="c0c7a-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="c0c7a-104">Sử dụng mô-đun Azure AD PowerShell-</span><span class="sxs-lookup"><span data-stu-id="c0c7a-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="c0c7a-105">Tham khảo: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="c0c7a-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="c0c7a-106">Sử dụng Azure CLI- `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="c0c7a-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="c0c7a-107">Tham khảo: [chủ sở hữu ứng dụng AZ AD](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="c0c7a-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="c0c7a-108">Sử dụng biểu đồ MS-</span><span class="sxs-lookup"><span data-stu-id="c0c7a-108">Using MS Graph -</span></span>

    <span data-ttu-id="c0c7a-109">Tham khảo: [Thêm chủ sở hữu-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="c0c7a-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="c0c7a-110">Sử dụng cổng thông tin Azure AD-dẫn hướng đến [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > ứng dụng đăng ký > chọn ứng dụng của bạn > chủ sở hữu > thêm chủ sở hữu</span><span class="sxs-lookup"><span data-stu-id="c0c7a-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="c0c7a-111">**Không thể xem ứng dụng của bạn trên lưỡi đăng ký ứng dụng, mặc dù bạn là chủ sở hữu ứng dụng đó?**</span><span class="sxs-lookup"><span data-stu-id="c0c7a-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="c0c7a-112">Chủ sở hữu ứng dụng không phải là vai trò quản trị.</span><span class="sxs-lookup"><span data-stu-id="c0c7a-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="c0c7a-113">Nếu thiết đặt [hạn chế quyền truy nhập vào cổng thông tin quản trị AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) sẽ được bật, thì người quản trị chỉ có thể xem các ứng dụng trên cổng đăng ký ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="c0c7a-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="c0c7a-114">Đối với người sở hữu có thể xem các ứng dụng, hãy tắt thiết đặt này (đặt điều này thành không) hoặc gán vai trò quản trị cho chủ sở hữu chỉ dành riêng cho ứng dụng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="c0c7a-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="c0c7a-115">Tuy nhiên, đối với điều này, bạn sẽ yêu cầu giấy phép Azure AD Premium P2 và bật [quản lý định danh đặc quyền](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span><span class="sxs-lookup"><span data-stu-id="c0c7a-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
