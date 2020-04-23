---
title: 932 nâng cấp AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766515"
---
# <a name="upgrade-azure-ad-connect"></a>Nâng cấp Azure AD kết nối

Theo mặc định, tính năng nâng cấp tự động được bật cho Azure AD Connect, giúp đảm bảo bạn đang chạy phiên bản mới nhất. Để xác minh cài đặt tự động nâng cấp, sử dụng lệnh **Get-ADSyncAutoUpgrade** Azure AD PowerShell. Lệnh này sẽ trả về một trong các giá trị sau:

- **Kích hoạt**: tự động nâng cấp được kích hoạt.

- **Vô hiệu hoá**: tự động nâng cấp bị vô hiệu hoá.

- Bị **tạm ngưng**: Hệ thống không còn đủ điều kiện để nhận các nâng cấp tự động. Bạn không thể cấu hình giá trị này; nó được thiết lập bởi hệ thống.

Để biết thêm thông tin, xem [nâng cấp tự động](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Để tải xuống phiên bản mới nhất của Azure AD kết nối [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594), hãy chuyển đến.
