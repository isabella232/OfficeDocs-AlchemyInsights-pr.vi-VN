---
title: Truy nhập có điều kiện với InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807681"
---
# <a name="conditional-access-with-intune"></a>Truy nhập có điều kiện với InTune

Sử dụng  **quyền truy nhập**  có điều kiện với InTune đòi hỏi phải có 3 bước:

- Tạo  **chính sách tuân thủ**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) để xác định các thiết đặt phải được đáp ứng trước khi thiết bị được xem là tuân thủ. Ví dụ: một thiết bị phải có mã pin của ít nhất 6 chữ số trước khi nó được xem là compliant.
- Tạo một **chính sách truy nhập**  có điều kiện xác định những tài nguyên đang được bảo vệ và điều kiện nào cần được đáp ứng để truy nhập các tài nguyên đó.  Ví [dụ:](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) thiết bị phải tuân thủ trước khi truy nhập email công ty.
- Đảm bảo cả **chính sách tuân thủ**  và  **chính sách truy nhập**  có điều kiện được nhắm vào các nhóm bạn muốn của người dùng. Điều này có thể yêu cầu tạo các nhóm người dùng cụ thể trong Azure Active Directory.

**Liên kết hữu ích:**

[Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)

[Khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Chính sách khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Để bảo vệ email (Exchange Online) từ Access bằng các thiết bị không tuân thủ, cả hai tài liệu đều phải được theo dõi:

1. [Bảo vệ truy nhập email từ các thiết bị bằng cách dùng EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Bảo vệ truy nhập email từ các thiết bị bằng cách dùng các máy khách xác thực hiện đại như Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)