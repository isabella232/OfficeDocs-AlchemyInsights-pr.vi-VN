---
title: Di chuyển thư email đến hộp thư Lưu trữ
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974979"
---
# <a name="move-email-to-the-archive-mailbox"></a>Di chuyển email đến hộp thư lưu trữ

Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các cài đặt được đề cập dưới đây, hãy chọn nút quay lại <-- ở đầu trang này, rồi nhập địa chỉ email của người dùng gặp sự cố khi di chuyển email đến hộp thư lưu trữ của họ.

1. Xác nhận rằng **hộp thư Lưu trữ** đã được kích hoạt. Nếu không, hãy sử dụng các bước trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) để bật hộp thư lưu trữ.

2. Để tự động lưu trữ thư vào  hộp thư lưu trữ, thẻ duy trì có hành động Di chuyển đến lưu trữ phải được đặt để tự động áp dụng cho toàn bộ hộp thư **(mặc định).** Sử dụng các bước ở đây để tạo thẻ: Thẻ [mặc định lưu trữ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tiếp theo, hãy thêm thẻ **Lưu trữ** vào chính sách duy trì của bạn. Trong trung Exchange quản trị Chính sách Duy trì, chọn Chính sách **>** thêm thẻ Di chuyển đến **Lưu** trữ vào chính > **Lưu.**

4. Bây [giờ Gán Chính sách Duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư của người dùng cụ thể. Chính sách tương tự sẽ được áp dụng cho cả **hộp thư** Chính và hộp **thư Lưu** trữ.

Có thể việc bắt buộc Trợ lý Thư mục được Quản lý (MFA) chạy và áp dụng các cài đặt mới cho hộp thư của người dùng. Chạy lệnh sau đây trong khi [kết nối với EXO PowerShell để](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) khởi động Trợ lý Thư mục được Quản lý cho một hộp thư cụ thể:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Để biết thêm thông tin về việc thiết lập chính sách lưu trữ, hãy xem mục Thiết lập chính sách lưu [trữ và xóa cho hộp thư.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  