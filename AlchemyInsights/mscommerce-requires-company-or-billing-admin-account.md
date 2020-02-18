---
title: Kết nối với mô-đun MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093656"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce yêu cầu tài khoản quản trị viên công ty hoặc thanh toán

Mô-đun MSCommerce yêu cầu tài khoản với công ty hoặc đặc quyền quản trị viên thanh toán. Nếu bạn nhận được lỗi sau, bạn sẽ cần phải kết nối lại với một tài khoản khác.

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

Nếu tài khoản của bạn không có đặc quyền công ty hoặc quản trị viên thanh toán, hãy liên hệ với quản trị viên CNTT của bạn.
