---
title: Kết nối vào mô-đun MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974697"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce yêu cầu tài khoản Người quản trị Công ty hoặc Người quản trị Thanh toán

Mô-đun MSCommerce yêu cầu tài khoản với đặc quyền của Công ty hoặc Người quản trị Thanh toán. Nếu bạn đang gặp phải lỗi sau đây, bạn sẽ cần phải kết nối lại với một tài khoản khác.

*ErrorMessage - Máy chủ từ xa trả về lỗi: (403) Cấm. ErrorDetails - Tại C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : Không xác định: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Nếu tài khoản của bạn không có đặc quyền Của công ty hoặc Người quản trị Thanh toán, hãy liên hệ với Người quản trị CNTT.
