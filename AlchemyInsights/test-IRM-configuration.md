---
title: Kiểm tra Cấu hình IRM cho các chức năng OME mới
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 22430e2b8a00023f9922fd59d6fcabd308d08453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317254"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Kiểm tra Cấu hình IRM cho các chức năng OME mới

Để xác minh rằng đối tượng thuê Microsoft 365 của bạn được đặt cấu hình để sử dụng các chức năng OME mới, hãy chạy lệnh ghép ngắn sau đây trong khi [kết nối với Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell)


1. Kiểm tra cấu hình IRM của đối tượng thuê của bạn bằng cách chạy `Get-IRMConfiguration` . Hãy đảm bảo rằng các giá trị này được đặt thành **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Sử dụng tên miền, địa chỉ người gửi và người nhận của bạn, chạy `Test-IRMConfiguration` . Nếu kiểm tra không đạt, hãy điều tra cấu hình IRM của bạn.

Để biết thêm thông tin về cách xác minh cấu hình IRM, xem mục Xác minh cấu hình [OME mới Exchange Online với PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)