---
title: ATP cho SharePoint, OneDrive và Microsoft nhóm
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715583"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP cho SharePoint, OneDrive và Microsoft nhóm

Làm theo các bước sau để bật tính năng bảo vệ mối đe dọa nâng cao:

1. Đi đến [https://protection.office.com](https://protection.office.com) và đăng nhập bằng tài khoản người quản trị toàn cầu hoặc người quản trị bảo mật.

2. Trong ngăn dẫn hướng bên trái bên dưới **quản lý mối đe dọa**, hãy chọn **chính sách** \> **tệp đính kèm an toàn**.

3. Chọn **bật ATP cho SharePoint, OneDrive và Microsoft nhóm**.

4. [Tạo một chính sách cảnh báo hoạt động](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) để nhận thông báo khi chúng tôi phát hiện tệp độc hại.

Để biết hướng dẫn đầy đủ, hãy xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)này.

**Lưu ý**: theo thiết kế, ATP không quét tất cả tệp duy nhất trong SharePoint Online, OneDrive for Business hoặc Microsoft nhóm. Các tệp được quét asynchronously theo quy trình sử dụng tính năng chia sẻ hoạt động, hoạt động của khách và các tín hiệu mối đe dọa để xác định các tệp độc hại. Để biết thêm thông tin, hãy xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)này.
