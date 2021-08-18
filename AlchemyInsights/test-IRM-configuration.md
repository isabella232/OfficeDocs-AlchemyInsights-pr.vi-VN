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
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899718"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Kiểm tra Cấu hình IRM cho các chức năng OME mới

Để xác minh rằng đối tượng thuê Microsoft 365 của bạn được cấu hình để sử dụng các chức năng OME mới, hãy chạy lệnh ghép ngắn sau đây trong khi [kết nối Exchange Online với PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell)


1. Kiểm tra cấu hình IRM của đối tượng thuê của bạn bằng cách chạy `Get-IRMConfiguration` . Hãy đảm bảo rằng các giá trị này được đặt thành **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Sử dụng tên miền, địa chỉ người gửi và người nhận của bạn, chạy `Test-IRMConfiguration` . Nếu kiểm tra không đạt, hãy điều tra cấu hình IRM của bạn.

Để biết thêm thông tin về cách xác minh cấu hình IRM, hãy xem xác minh cấu hình [OME mới Exchange Online PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)