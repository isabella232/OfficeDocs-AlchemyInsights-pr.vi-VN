---
title: Tự động mã hóa Office 365 email được gửi đến một số tên miền nhất định
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082208"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Tự động mã hóa Office 365 email được gửi đến một số tên miền nhất định

1. Từ trung [Exchange quản trị Viên](https://outlook.office365.com/ecp/), chọn quy tắc dòng > **thư.** 
2. Bấm vào **biểu tượng Mới (+),** rồi bấm vào Áp **dụng Mã hóa Thư Office 365 và bảo vệ quyền cho thư.**
3. Trong **Tên**, hãy nhập tên cho quy tắc, chẳng hạn như Mã hóa *thư được gửi đến contoso.com.*
4. Trong **Áp dụng quy tắc này nếu**, chọn Người > **là**. 
5. Nhập tên miền, chẳng hạn như **contoso.com.**
6. Bấm vào **biểu tượng Thêm (+),** rồi bấm **OK.**
7. Bên cạnh trường **Thực hiện như sau,** bấm vào **Chọn một mục**. 
8. Trong menu **thả xuống mẫu RMS,** chọn Mã **hóa**, rồi bấm **OK.** (Nếu bạn không thấy tùy chọn này, có nghĩa là gói của bạn không bao gồm mã hóa tự động. Nhưng bạn có thể thêm nó!)
9. Chọn bất kỳ lựa chọn tùy chọn nào (từ danh sách các lựa chọn tùy chọn mà bạn có thể thực hiện tại thời điểm này, nhiều lựa chọn trong số đó có thể được để lại cài đặt mặc định cho đơn giản).
10. Bấm vào **Lưu**.

> [!IMPORTANT]
> Sau này, bạn luôn có thể quay lại và chỉnh sửa quy tắc này.

Để biết thêm thông tin về cách tạo quy tắc mã hóa, xem mục Xác [định quy tắc dòng thư để mã hóa thư email Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)