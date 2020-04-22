---
title: Cho phép Office 365 ATP dành cho SharePoint, OneDrive và Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703448"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Cho phép Office 365 nâng cao mối đe dọa bảo vệ cho SharePoint trực tuyến, OneDrive và Microsoft teams

1. Đi tới https://protection.office.com và đăng nhập.
2. Chọn **mối đe dọa quản lý** > **chính sách** > **đính kèm an toàn**.
3. Chọn **bật ATP cho SharePoint, OneDrive và Microsoft teams**, sau đó bấm vào **lưu**.
4. Khuyến cáo Là quản trị viên toàn cầu hoặc quản trị viên SharePoint trực tuyến, chạy lệnh ghép ngắn [Set-Spothuê](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **Disallowinfectedfiledownload** đặt *đúng*.
5. Khuyến cáo [Thiết lập cảnh báo](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tệp được phát hiện.

> [!NOTE]
> ATP sẽ NTO quét mọi tệp duy nhất trong SharePoint Online, OneDrive hoặc Microsoft teams. Tập tin được quét không đồng bộ, thông qua một quá trình sử dụng chia sẻ và các sự kiện hoạt động khách, cùng với thông minh chẩn đoán và mối đe dọa tín hiệu để xác định các tập tin độc hại. Xem [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)nào.