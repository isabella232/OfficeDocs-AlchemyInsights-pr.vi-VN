---
title: Chính sách Duy trì trong Trung tâm Quản trị Exchange không hoạt động
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952250"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Chính sách Duy trì trong Trung tâm Quản trị Exchange

Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các cài đặt được đề cập dưới đây, hãy chọn nút quay lại <-- ở đầu trang này, rồi nhập địa chỉ email của người dùng gặp sự cố với chính sách duy trì.

Nếu bạn gặp sự cố với chính sách duy trì trong Trung tâm Quản trị Exchange không áp dụng cho hộp thư hoặc các mục không di chuyển đến hộp thư lưu trữ, hãy kiểm tra các mục sau:

**Nguyên nhân gốc:**

- **Bộ trợ giúp Thư mục có** Quản lý chưa xử lý hộp thư của người dùng. Trợ lý Thư mục có Quản lý cố gắng xử lý mỗi hộp thư trong tổ chức trên nền điện toán đám mây của bạn một lần bảy ngày một lần.

  **Giải pháp:** Chạy Bộ trợ giúp Thư mục có Quản lý.

- **RetentionHold** đã được **bật trên** hộp thư. Nếu hộp thư đã được đặt trên Giữ lại, chính sách duy trì trên hộp thư sẽ không được xử lý trong thời gian đó.

  **Giải pháp:** Kiểm tra trạng thái của cài đặt Giữ lại và cập nhật nếu cần. Để biết chi tiết, hãy xem [Giữ lại Hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Lưu ý:** Nếu một hộp thư nhỏ hơn 10 MB, Trợ lý Thư mục được Quản lý sẽ không tự động xử lý hộp thư đó.
 
Để biết thêm thông tin về chính sách duy trì trong Trung tâm Quản trị Exchange, hãy xem:

- [Thẻ duy trì và chính sách duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Áp dụng chính sách duy trì cho hộp thư hoặc](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Thêm hoặc loại bỏ thẻ duy [trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Cách xác định loại giữ được đặt trên hộp thư](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
