---
title: Di chuyển thư email đến hộp thư lưu trữ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511062"
---
# <a name="move-email-to-the-archive-mailbox"></a>Di chuyển email đến hộp thư lưu trữ

1. Xác nhận rằng **hộp thư lưu trữ** đã được bật. Nếu không, sử dụng các bước trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) để kích hoạt hộp thư lưu trữ.

2. Để lưu trữ thư tự động vào hộp thư lưu trữ, thẻ lưu giữ với hành động **di chuyển đến lưu trữ** phải được đặt **tự động áp dụng cho toàn bộ thẻ hộp thư (mặc định)**. Sử dụng các bước ở đây để tạo thẻ: [lưu trữ thẻ mặc định](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Tiếp theo, thêm thẻ **lưu trữ** vào chính sách lưu giữ của bạn. Trong Trung tâm quản trị Exchange, chọn **chính sách lưu giữ** > thêm **di chuyển vào thẻ lưu trữ** chính sách > **lưu**.

4. Bây giờ [chỉ định chính sách lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư của người dùng cụ thể. Chính sách tương tự sẽ được áp dụng cho cả hộp thư **chính** và **lưu trữ** .

Nó có thể là cần thiết để buộc quản lý thư mục hỗ trợ (MFA) để chạy và áp dụng cài đặt mới cho hộp thư của người dùng. Chạy lệnh sau khi [kết nối với eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) khởi động hỗ trợ thư mục được quản lý cho một hộp thư cụ thể:
  
Bắt đầu-ManagedFolderAssistant-Identity<name of the mailbox>

Để biết thêm thông tin về cách thiết lập chính sách lưu trữ, xem [thiết lập chính sách lưu trữ và xóa cho hộp thư](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  