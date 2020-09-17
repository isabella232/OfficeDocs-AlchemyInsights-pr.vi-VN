---
title: Di chuyển thư email đến hộp thư lưu trữ
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799802"
---
# <a name="move-email-to-the-archive-mailbox"></a>Di chuyển email đến hộp thư lưu trữ

Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các thiết đặt được đề cập dưới đây, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của người dùng có vấn đề chuyển email đến hộp thư lưu trữ của họ.

1. Xác nhận rằng **hộp thư lưu trữ** đã được bật chưa. Nếu không, hãy làm theo các bước trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) để cho phép hộp thư lưu trữ.

2. Để tự động lưu trữ thư vào hộp thư lưu trữ, thẻ duy trì với hành động **di chuyển đến lưu trữ** phải được đặt **tự động áp dụng cho toàn bộ hộp thư (mặc định)**. Hãy làm theo các bước sau đây để tạo thẻ: [thẻ mặc định lưu trữ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tiếp theo, thêm thẻ **lưu trữ** vào chính sách duy trì của bạn. Trong Trung tâm quản trị Exchange, hãy chọn **chính sách duy trì** > thêm **thẻ lưu vào thẻ lưu trữ** vào chính sách > **lưu**.

4. Bây giờ, [gán chính sách duy trì](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư của người dùng cụ thể. Chính sách này sẽ được áp dụng cho cả **chính** và hộp thư **lưu trữ** .

Có thể cần phải có hiệu lực trợ lý thư mục được quản lý (MFA) để chạy và áp dụng các thiết đặt mới cho hộp thư của người dùng. Chạy lệnh sau đây khi được [kết nối với EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) để khởi động trợ lý thư mục được quản lý cho một hộp thư cụ thể:
  
Khởi động-ManagedFolderAssistant-Identity <name of the mailbox>

Để biết thêm thông tin về việc thiết lập chính sách lưu trữ, hãy xem [thiết lập chính sách lưu trữ và xóa cho hộp thư](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  