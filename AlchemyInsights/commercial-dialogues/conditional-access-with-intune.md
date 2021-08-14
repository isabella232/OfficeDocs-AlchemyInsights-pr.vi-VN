---
title: Sử dụng quyền truy nhập có điều kiện với Intune
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
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005796"
---
# <a name="using-conditional-access-with-intune"></a>Sử dụng quyền truy nhập có điều kiện với Intune

Cần thực hiện 3 bước để sử dụng Quyền truy nhập có điều kiện với Intune:

- [Tạo một Chính sách tuân thủ để xác định các cài đặt phải được đáp ứng trước khi thiết bị được coi là đã tuân thủ. Ví dụ: thiết bị phải có mã pin tối thiểu 6 chữ số trước khi được coi là đã tuân thủ.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Tạo một Chính sách truy nhập có điều kiện xác định tài nguyên được bảo vệ và những điều kiện cần đáp ứng để truy nhập các tài nguyên đó. Ví dụ: thiết bị phải tuân thủ trước khi truy nhập email công ty.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Đảm bảo cả Chính sách tuân thủ và Chính sách truy nhập có điều kiện đều hướng đến nhóm người dùng mong muốn. Có thể cần tạo nhóm người dùng cụ thể trong Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Đọc thêm...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
