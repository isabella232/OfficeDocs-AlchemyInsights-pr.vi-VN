---
title: Kích hoạt Office 365 ATP cho SharePoint, OneDrive và Microsoft đội
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403055"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Sử Office 365 nâng cao mối đe dọa bảo vệ cho SharePoint trực tuyến, OneDrive và Microsoft đội

1. Đi đến https://protection.office.com và đăng nhập.
2. Chọn **quản lý mối đe dọa** > **chính sách** > **Tập tin đính kèm an toàn**.
3. Chọn **bật ATP cho Microsoft đội, SharePoint và OneDrive,** và sau đó nhấp vào **lưu**.
4. (Khuyến cáo) Như là một quản trị toàn cầu hoặc quản trị viên SharePoint Online, chạy lệnh ghép ngắn [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **DisallowInfectedFileDownload** được đặt thành *true*.
5. (Khuyến cáo) [Thiết lập cảnh báo](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tập tin được phát hiện.

> [!NOTE]
> ATP sẽ nto quét mỗi tập tin trong SharePoint Online, OneDrive hoặc Microsoft Teams. Tập tin được quét không đồng bộ, thông qua một quá trình sử dụng chia sẻ và khách hoạt động sự kiện, cùng với các chẩn đoán thông minh và mối đe dọa tín hiệu để xác định các tập tin độc hại. Xem [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).