---
title: Tự động mã hóa các thư email Office 365 được gửi đến một số tên miền
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749295"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Tự động mã hóa các thư email Office 365 được gửi đến một số tên miền

1. Từ [Trung tâm quản trị Exchange](https://outlook.office365.com/ecp/), chọn **quy tắc > dòng thư**. 
2. Bấm vào biểu tượng **(+) mới** , rồi bấm vào **áp dụng mã hóa thư Office 365 và bảo vệ quyền đối với thư**.
3. Trong **tên**, hãy nhập tên cho quy tắc, chẳng hạn như *mã hóa thư được gửi đến contoso.com*.
4. Trong **áp dụng quy tắc này nếu**, chọn **miền > người nhận là**. 
5. Nhập tên miền, chẳng hạn như **contoso.com**.
6. Bấm vào biểu tượng **Thêm (+)** , rồi bấm **OK**.
7. Bên cạnh trường **thực hiện các bước sau** , hãy bấm **chọn một**. 
8. Trong menu thả xuống của **mẫu RMS** , chọn **mã hóa**, rồi bấm **OK**. (Nếu bạn không thấy tùy chọn này, có nghĩa là gói đăng ký của bạn không bao gồm mã hóa tự động. Tuy nhiên, bạn có thể thêm nó!
9. Chọn bất kỳ lựa chọn tùy chọn nào (từ danh sách các lựa chọn tùy chọn mà bạn có thể thực hiện tại thời điểm này, nhiều phần có thể còn lại với cài đặt mặc định cho đơn giản hơn).
10. Bấm vào **Lưu**.

> [!IMPORTANT]
> Bạn luôn có thể quay lại và chỉnh sửa quy tắc này sau này.

Để biết thêm thông tin về cách tạo quy tắc cho mã hóa, hãy xem mục [xác định quy tắc dòng thư để mã hóa thư email trong Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)