---
title: Truy nhập có điều kiện với Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069734"
---
# <a name="conditional-access-with-intune"></a>Truy nhập có điều kiện với Intune

Cần thực  **hiện 3 bước**  để sử dụng Quyền truy nhập có điều kiện với Intune:

- Tạo một Chính **sách tuân thủ** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) để xác định các cài đặt phải được đáp ứng trước khi thiết bị được coi là đã tuân thủ. Ví dụ: thiết bị phải có mã pin tối thiểu 6 chữ số trước khi được coi là đã tuân thủ.
- Tạo một Chính **sách truy nhập có điều kiện**  xác định tài nguyên được bảo vệ và những điều kiện cần đáp ứng để truy nhập các tài nguyên đó.  [Ví dụ: thiết](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  bị phải tuân thủ trước khi truy nhập email công ty.
- Đảm bảo cả **Chính sách tuân thủ**  và Chính sách truy nhập có  **điều**  kiện đều hướng đến nhóm người dùng mong muốn. Có thể cần tạo nhóm người dùng cụ thể trong Azure Active Directory.

**Các liên kết hữu ích:**

[Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)

[Khắc phục sự cố CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Chính sách khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Để bảo vệ Email (Exchange trực tuyến) khỏi truy nhập bằng các thiết bị không tương thích, bạn phải tuân theo cả hai tài liệu này:

1. [Bảo vệ quyền truy nhập email từ thiết bị bằng EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Bảo vệ quyền truy nhập email khỏi các thiết bị bằng máy khách xác thực hiện đại như Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)