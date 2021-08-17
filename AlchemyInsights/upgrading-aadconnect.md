---
title: 932 Nâng cấp AADConnect
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104834"
---
# <a name="upgrade-azure-ad-connect"></a>Nâng cấp Azure AD Kết nối

Theo mặc định, tự động nâng cấp được bật cho Azure AD Kết nối, giúp đảm bảo bạn đang chạy phiên bản mới nhất. Để xác minh cài đặt nâng cấp tự động, hãy sử dụng lệnh ghép ngắn **Get-ADSyncAutoUpgrade** trong Azure AD PowerShell. Lệnh ghép ngắn sẽ trả về một trong các giá trị sau:

- **Đã bật**: Đã bật tự động nâng cấp.

- **Đã tắt:** Tự động nâng cấp bị vô hiệu hóa.

- **Đã tạm ngừng**: Hệ thống không còn đủ điều kiện nhận các bản nâng cấp tự động nữa. Bạn không thể cấu hình giá trị này; do hệ thống đặt.

Để biết thêm thông tin, hãy xem [mục Nâng cấp tự động.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Để tải xuống phiên bản mới nhất của Azure AD Kết nối, hãy đi tới [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
