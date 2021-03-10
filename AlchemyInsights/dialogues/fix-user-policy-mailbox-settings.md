---
title: Sửa chữa chính sách/thiết đặt hộp thư của người dùng
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695896"
---
# <a name="fix-user-policymailbox-settings"></a>Sửa chữa chính sách/thiết đặt hộp thư của người dùng

Thiết đặt thư rác trên hộp thư ảnh hưởng đến thư này. Để xem lại các cài đặt, hãy làm như sau:

1. Khởi động Exchange Management Shell. Để biết thêm thông tin, hãy xem [mở Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Chạy lệnh này (sử dụng địa chỉ email của người dùng):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**
3. Kiểm tra xem địa chỉ email của người gửi là một phần trong **Trustedsendersanddomains** hay **Blockenhsendersanddomains**. Nếu địa chỉ email nằm trong một trong các danh sách, bạn có thể phải loại bỏ nó. Để tìm hiểu thêm, hãy xem [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
