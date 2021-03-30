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
# <a name="app-registration-owner-issues"></a>Vấn đề về chủ sở hữu đăng ký ứng dụng

Sau đây là các phương pháp sẵn dùng để thêm hiệu trưởng với tư cách là chủ sở hữu cho đăng ký ứng dụng:

- Sử dụng mô-đun Azure AD PowerShell-

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Tham khảo: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Sử dụng Azure CLI- `az ad app owner add`

    Tham khảo: [chủ sở hữu ứng dụng AZ AD](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Sử dụng biểu đồ MS-

    Tham khảo: [Thêm chủ sở hữu-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Sử dụng cổng thông tin Azure AD-dẫn hướng đến [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > ứng dụng đăng ký > chọn ứng dụng của bạn > chủ sở hữu > thêm chủ sở hữu

**Không thể xem ứng dụng của bạn trên lưỡi đăng ký ứng dụng, mặc dù bạn là chủ sở hữu ứng dụng đó?**

Chủ sở hữu ứng dụng không phải là vai trò quản trị. Nếu thiết đặt [hạn chế quyền truy nhập vào cổng thông tin quản trị AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) sẽ được bật, thì người quản trị chỉ có thể xem các ứng dụng trên cổng đăng ký ứng dụng. Đối với người sở hữu có thể xem các ứng dụng, hãy tắt thiết đặt này (đặt điều này thành không) hoặc gán vai trò quản trị cho chủ sở hữu chỉ dành riêng cho ứng dụng cụ thể. Tuy nhiên, đối với điều này, bạn sẽ yêu cầu giấy phép Azure AD Premium P2 và bật [quản lý định danh đặc quyền](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
