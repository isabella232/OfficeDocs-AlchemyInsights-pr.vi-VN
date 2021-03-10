---
title: Sử dụng quyền truy nhập có điều kiện với InTune
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694719"
---
# <a name="using-conditional-access-with-intune"></a>Sử dụng quyền truy nhập có điều kiện với InTune

Sử dụng quyền truy nhập có điều kiện với InTune đòi hỏi phải có 3 bước:

- [Tạo chính sách tuân thủ để xác định các thiết đặt phải được đáp ứng trước khi thiết bị được xem là tuân thủ. Ví dụ: một thiết bị phải có mã pin của ít nhất 6 chữ số trước khi nó được xem là compliant.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Tạo một chính sách truy nhập có điều kiện xác định những tài nguyên đang được bảo vệ và điều kiện nào cần được đáp ứng để truy nhập các tài nguyên đó. Ví dụ: thiết bị phải tuân thủ trước khi truy nhập email công ty.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Đảm bảo cả chính sách tuân thủ và chính sách truy nhập có điều kiện được nhắm vào các nhóm bạn muốn của người dùng. Điều này có thể yêu cầu tạo các nhóm người dùng cụ thể trong Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Đọc thêm...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
