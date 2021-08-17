---
title: Bật Két sắt kèm cho mọi SharePoint Online, OneDrive và Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894485"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Bật Két sắt kèm cho mọi SharePoint Online, OneDrive và Microsoft Teams

1. Sử dụng thông tin xác thực người quản trị toàn cầu hoặc người quản trị bảo mật của bạn, mở cổng thông tin Bộ bảo vệ Microsoft 365 tại , rồi đi đến Chính sách & Quy tắc chính sách mối đe <https://security.microsoft.com>  \>  \> **dọa**  sẽ Két sắt Phần đính kèm trong phần Chính sách

   Để đi thẳng tới trang **Két sắt Đính kèm,** sử dụng <https://security.microsoft.com/safeattachmentv2> .

2. Trên trang Phần **Két sắt kèm,** bấm Thiết **đặt chung.**
3. Trên hộp bật ra xuất hiện, chọn Bật Bộ bảo vệ Microsoft cho Office 365 cho **SharePoint, OneDrive và Microsoft Teams**, sau đó chọn **Lưu**.

    > [!TIP]
    >
    > Thực hiện các bước sau đây để tăng cường bảo vệ Két sắt Tệp đính kèm cho SharePoint, OneDrive tệp và Microsoft Teams:
    >
    > - Để ngăn người dùng tải xuống các tệp độc hại, hãy sử dụng giá trị cho tham số `$true` *DisallowInfectedFileDownload* trên lệnh ghép ngắn **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** trong SharePoint Online PowerShell. Để biết thêm thông [tin, hãy xem SharePoint Online PowerShell](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)để ngăn người dùng tải xuống các tệp độc hại.
    > - [Tạo chính sách cảnh báo cho các tệp được phát hiện](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Để biết thêm thông tin, hãy xem Két sắt xem Phần đính [Office 365 để biết SharePoint, OneDrive và Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
