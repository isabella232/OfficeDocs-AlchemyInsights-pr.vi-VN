---
title: Bật Bộ bảo vệ Microsoft dành Office 365 cho SharePoint Online, OneDrive và Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058888"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Bật Bộ bảo vệ Microsoft dành Office 365 cho SharePoint Online, OneDrive và Microsoft Teams

1. Sử dụng thông tin xác thực người quản trị toàn cầu hoặc người quản trị bảo mật của bạn, đăng [nhập vào Office 365 tâm Bảo mật và Tuân thủ](https://protection.office.com/).
2. Chọn **Quản lý mối đe** dọa trong ngăn bên trái, rồi chọn Chính sách **Két sắt**  >  [kèm](https://protection.office.com/safeattachment).
3. Chọn **Bật Bộ bảo vệ Microsoft cho Office 365 cho SharePoint, OneDrive và Microsoft Teams**, sau đó chọn **Lưu**.
    > [!TIP]
    >
    > - Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn PowerShell sau đây với tham số **DisallowInfectedFileDownload** được đặt thành *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Thiết lập cảnh báo cho các tệp được phát hiện](https://go.microsoft.com/fwlink/?linkid=2092110)

Để biết thêm thông tin, xem [mục Bộ bảo vệ Microsoft Office 365 để biết SharePoint, OneDrive và Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
