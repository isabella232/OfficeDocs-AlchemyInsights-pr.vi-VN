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
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812451"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Kiểm tra Cấu hình IRM cho các chức năng OME mới

Để xác minh rằng đối tượng thuê Microsoft 365 của bạn đã được cấu hình để sử dụng các chức năng OME mới, hãy chạy lệnh ghép ngắn sau đây trong khi [kết nối Exchange Online với PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Kiểm tra cấu hình IRM của đối tượng thuê của bạn bằng cách chạy `Get-IRMConfiguration` . Hãy đảm bảo rằng các giá trị này được đặt thành **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Sử dụng tên miền, địa chỉ người gửi và người nhận của bạn, chạy `Test-IRMConfiguration` . Nếu kiểm tra không đạt, hãy điều tra cấu hình IRM của bạn.

Để biết thêm thông tin về cách xác minh cấu hình IRM, xem mục Xác minh cấu hình [OME mới Exchange Online với PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)