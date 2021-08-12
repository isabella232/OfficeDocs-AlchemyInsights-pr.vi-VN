---
title: Các sự cố về Chủ sở hữu Đăng ký Ứng dụng
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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951155"
---
# <a name="app-registration-owner-issues"></a>Các sự cố về Chủ sở hữu Đăng ký Ứng dụng

Sau đây là các phương thức có sẵn để thêm tên chính làm chủ sở hữu đối với đăng ký ứng dụng:

- Sử dụng Mô-đun Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Tham khảo: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Sử dụng Azure CLI - `az ad app owner add`

    Tham khảo: [chủ sở hữu ứng dụng quảng cáo az](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Đang sử dụng MS Graph -

    Tham khảo: [Thêm chủ sở hữu - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Sử dụng Cổng thông tin Azure AD - Dẫn hướng đến [portal.azure.com](https://portal.azure.com/) > Đăng ký Ứng dụng Azure Active directory > > Chọn chủ sở hữu ứng dụng > để > thêm chủ sở hữu

**Không thể xem ứng dụng của bạn trên lưỡi Đăng ký Ứng dụng ngay cả khi bạn là chủ sở hữu của ứng dụng đó?**

Chủ sở hữu ứng dụng không phải là vai trò quản trị. Nếu thiết đặt [Hạn chế quyền truy](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) nhập vào cổng thông tin quản trị Azure AD được bật thì chỉ người quản trị mới có thể xem các ứng dụng trên cổng thông tin Đăng ký Ứng dụng. Để chủ sở hữu có thể xem các ứng dụng, hãy tắt thiết đặt này (Đặt thiết đặt này thành KHÔNG) hoặc gán vai trò quản trị cho chủ sở hữu chỉ đối với ứng dụng cụ thể. Tuy nhiên, để thực hiện điều này, bạn sẽ cần có giấy phép Azure AD Premium P2 và [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
