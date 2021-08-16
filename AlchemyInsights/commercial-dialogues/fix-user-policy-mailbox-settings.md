---
title: Khắc phục cài đặt chính sách người dùng/hộp thư
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034740"
---
# <a name="fix-user-policymailbox-settings"></a>Khắc phục cài đặt chính sách người dùng/hộp thư

Thiết đặt thư rác trên hộp thư đã ảnh hưởng đến thư này. Để xem lại các thiết đặt, hãy làm như sau:

1. Khởi Exchange Management Shell. Để biết thêm thông tin, [hãy xem Mở Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Chạy lệnh này (sử dụng địa chỉ email của người dùng):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kiểm tra xem địa chỉ email của người gửi có phải là một phần của **TrustedSendersAndDomains** hoặc **BlockedSendersAndDomains hay không.** Nếu địa chỉ email nằm ở một trong các danh sách, bạn có thể phải loại bỏ địa chỉ đó. Để tìm hiểu thêm, [hãy xem Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
