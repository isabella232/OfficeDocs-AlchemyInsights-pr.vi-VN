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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527747"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Tự động di chuyển thư email đến hộp thư lưu trữ

Sau đây là cách thiết lập chính sách để tự động di chuyển email cũ của người dùng vào hộp thư lưu trữ:

1. Đi đến [**bảo mật &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **quản trị dữ liệu** tuân thủ  >   để xác nhận một hộp thư lưu trữ đã được kích hoạt cho người dùng. Nếu chưa có, hãy bấm **bật** sau đó **có** trong hộp cảnh báo.
2. Đi đến [**Trung tâm quản trị Exchange > quản lý tuân thủ > thẻ duy trì**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Chọn biểu tượng + sau đó chọn **tự động áp dụng cho toàn bộ hộp thư**.
4. Gán tên cho thẻ duy trì, rồi chọn **di chuyển đến lưu trữ**. Đối với khoảng thời gian lưu giữ, hãy nhập thời gian bạn muốn, chẳng hạn như 90 ngày. Bấm vào **Lưu**.
5. Bây giờ, tạo chính sách duy trì: chọn **chính sách duy trì**, chọn biểu tượng để thêm chính sách mới.
6. Gán tên cho chính sách duy trì, rồi bấm và cuộn để tìm và thêm thẻ duy trì mà bạn vừa tạo ra. Bấm vào **Lưu**.
7. Cuối cùng, áp dụng chính sách duy trì cho hộp thư của người dùng: vẫn trong Trung tâm quản trị Exchange, đi đến  >  **hộp thư** của người nhận. Chọn tất cả những người dùng bạn muốn áp dụng chính sách, rồi chọn **chỉnh sửa** (biểu tượng bút chì).
8. Trong hộp thoại, bấm vào **tính năng hộp thư**. Bên dưới **chính sách duy trì**, áp dụng chính sách mà bạn vừa tạo > **lưu**.
9. Để biết hướng dẫn về cách áp dụng chính sách cho tất cả người dùng, hãy xem [áp dụng chính sách duy trì cho hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
