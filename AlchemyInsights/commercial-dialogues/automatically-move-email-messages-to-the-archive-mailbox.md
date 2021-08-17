---
title: Tự động di chuyển thư email đến hộp thư lưu trữ
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
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059248"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Tự động di chuyển thư email đến hộp thư lưu trữ

Sau đây là cách thiết lập chính sách để tự động di chuyển email cũ của người dùng vào hộp thư lưu trữ:

1. Đi đến mục [**Bảo & quản trị**](https://go.microsoft.com/fwlink/p/?linkid=2077143)dữ liệu tuân thủ để xác minh rằng hộp thư lưu trữ đã được kích hoạt cho người  >    >   dùng. Nếu tính năng này chưa kích hoạt, hãy **bấm Bật** **rồi Có** trong hộp cảnh báo.
2. Đi đến trung [**Exchange quản trị viên để > thẻ duy > tuân thủ.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Chọn biểu tượng + rồi chọn tự động **áp dụng cho toàn bộ hộp thư.**
4. Gán tên cho thẻ duy trì, rồi chọn Di chuyển **đến Lưu trữ**. Đối với thời gian lưu giữ, hãy nhập thời gian bạn muốn, chẳng hạn như 90 ngày. Bấm vào **Lưu**.
5. Bây giờ hãy tạo một chính sách duy trì: **chọn chính sách duy** trì, chọn biểu tượng để thêm chính sách mới.
6. Gán tên cho chính sách duy trì, sau đó bấm và cuộn để tìm và thêm thẻ duy trì mà bạn vừa tạo ra. Bấm vào **Lưu**.
7. Cuối cùng, áp dụng chính sách duy trì cho hộp thư của người dùng: vẫn ở trong trung tâm quản trị Exchange của người nhận, **đi đến hộp thư** người  >  **nhận**. Chọn tất cả người dùng mà bạn muốn áp dụng chính sách, sau đó chọn **Chỉnh sửa** (biểu tượng bút chì).
8. Trong hộp thoại, bấm vào tính **năng hộp thư.** Bên dưới **Chính sách duy** trì , áp dụng chính sách mà bạn vừa tạo > **Lưu.**
9. Để biết hướng dẫn áp dụng chính sách cho tất cả người dùng, hãy [xem mục Áp dụng chính sách duy trì cho hộp thư.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
