---
title: Cho phép Office 365 ATP cho SharePoint, OneDrive và Microsoft nhóm
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801097"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Cho phép Microsoft Defender cho Office 365 cho SharePoint Online, OneDrive và Microsoft nhóm

1. Đi đến https://protection.office.com và đăng nhập.
2. Chọn chính sách **quản lý mối đe dọa**  >  **Policy**  >  **an toàn phần đính kèm** .
3. Chọn **bật ATP cho SharePoint, OneDrive và Microsoft nhóm** , rồi bấm **lưu** .
4. Quản Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn [Set-spođối](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với bộ tham số **tải xuống của Outallowinfectedfileto** *True* .
5. Quản [Thiết lập cảnh báo](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) cho các tệp đã phát hiện.

> [!NOTE]
> ATP sẽ NTO quét tất cả tệp đơn lẻ trong SharePoint Online, OneDrive hoặc Microsoft nhóm. Các tệp được quét asynchronously, qua một quy trình sử dụng các sự kiện hoạt động chia sẻ và khách, cùng với các tín hiệu thông minh và phản đối mối đe dọa để xác định các tệp độc hại. Xem [ATP cho SharePoint, OneDrive và Microsoft nhóm](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).