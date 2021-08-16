---
title: Xóa hoặc khôi phục ứng dụng
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102593"
---
# <a name="delete-or-restore-applications"></a>Xóa hoặc khôi phục ứng dụng

**Để xóa một ứng dụng khỏi đối tượng thuê Azure AD của bạn:**

1. Trong cổng thông **tin Azure AD**, chọn Ứng dụng doanh **nghiệp**. Sau đó tìm và chọn ứng dụng bạn muốn xóa.
2. Trong phần **Quản lý** ở ngăn bên trái, chọn Thuộc **tính.**
3. Chọn **Xóa**, rồi chọn Có **để xác** nhận bạn muốn xóa ứng dụng khỏi đối tượng thuê Azure AD của mình.

Để biết thêm thông tin về cách xóa ứng dụng, hãy xem Bắt đầu nhanh: Xóa một ứng dụng khỏi đối tượng thuê [Azure Active Directory (Azure AD) của bạn.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

Trong PowerShell, lệnh ghép ngắn [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) sẽ loại bỏ cấu hình Application Proxy khỏi một ứng dụng cụ thể trong Azure Active Directory và có thể xóa ứng dụng hoàn toàn nếu được chỉ định.

Bạn có thể **khôi phục ứng dụng đã xóa** bằng PowerShell. Sau khi ứng dụng bạn muốn khôi phục đã được xác định, bạn có thể khôi phục ứng dụng đó bằng cách sử dụng [Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
