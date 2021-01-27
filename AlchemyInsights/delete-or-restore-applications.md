---
title: Xóa hoặc khôi phục các ứng dụng
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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015023"
---
# <a name="delete-or-restore-applications"></a>Xóa hoặc khôi phục các ứng dụng

**Để xóa một ứng dụng khỏi AZURE AD đối tượng thuê của bạn**:

1. Trong **cổng thông tin AZURE AD**, chọn **ứng dụng doanh nghiệp**. Sau đó tìm và chọn ứng dụng mà bạn muốn xóa bỏ.
2. Trong phần **quản lý** trong ngăn bên trái, hãy chọn **thuộc tính**.
3. Chọn **xóa**, rồi chọn **có** để xác nhận bạn muốn xóa ứng dụng khỏi Azure AD đối tượng thuê của bạn.

Để biết thêm thông tin về cách xóa ứng dụng, hãy xem [bắt đầu nhanh: xóa một ứng dụng từ đối tượng thuê Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

Trong PowerShell, lệnh ghép ngắn [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) sẽ loại bỏ cấu hình proxy ứng dụng từ một ứng dụng cụ thể trong Azure Active Directory và có thể xóa ứng dụng hoàn toàn nếu được chỉ định.

Bạn có thể **khôi phục một ứng dụng đã xóa** bằng PowerShell. Sau khi ứng dụng mà bạn muốn khôi phục đã được xác định, bạn có thể khôi phục nó bằng cách dùng [khôi phục-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
