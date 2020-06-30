---
title: Truy cập có điều kiện với InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931458"
---
# <a name="conditional-access-with-intune"></a>Truy cập có điều kiện với InTune

Sử dụng **truy cập có điều kiện** với InTune yêu cầu 3 bước:

- Tạo **chính sách tuân thủ** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) để xác định cài đặt phải được đáp ứng trước khi thiết bị được coi là tuân thủ. Ví dụ: một thiết bị phải có một pin ít nhất 6 chữ số trước khi nó được coi là phù hợp.
- Tạo **chính sách truy cập có điều kiện** xác định tài nguyên nào đang được bảo vệ và điều kiện nào cần được đáp ứng để truy cập các tài nguyên đó.  Ví [dụ:](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) một thiết bị phải tuân thủ trước khi truy cập email công ty.
- Đảm bảo cả **chính sách tuân thủ** và **chính sách truy cập có điều kiện** đều được nhắm mục tiêu đến các nhóm người dùng mong muốn. Điều này có thể yêu cầu tạo nhóm người dùng cụ thể trong Azure Active Directory.

**Liên kết hữu ích:**

[Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)

[Khắc phục sự cố CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Chính sách khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Để bảo vệ email (Exchange Online) từ truy cập bởi các thiết bị noncompliant, cả hai tài liệu phải được tuân theo:

1. [Bảo vệ truy cập email từ các thiết bị sử dụng EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Bảo vệ truy cập email từ các thiết bị sử dụng các máy khách xác thực hiện đại như Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)