---
title: nâng cấp lên 932
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806061"
---
# <a name="upgrade-azure-ad-connect"></a>Nâng cấp kết nối Azure AD

Theo mặc định, nâng cấp tự động được bật cho Azure AD Connect, vốn sẽ giúp đảm bảo bạn đang chạy phiên bản mới nhất. Để xác minh cài đặt nâng cấp tự động, hãy sử dụng lệnh ghép ngắn **Get-ADSyncAutoUpgrade** trong Azure AD PowerShell. Lệnh ghép ngắn sẽ trả về một trong các giá trị sau:

- Đã **bật**: nâng cấp tự động được bật.

- **Tắt**: nâng cấp tự động bị vô hiệu hóa.

- Bị **tạm ngừng**: Hệ thống không còn đủ điều kiện để nhận các nâng cấp tự động. Bạn không thể cấu hình giá trị này; nó được đặt bởi hệ thống.

Để biết thêm thông tin, hãy xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Để tải xuống phiên bản mới nhất của Azure AD Connect, hãy đi tới [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
