---
title: 1336 RecoverableItems thư mục đầy đủ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720274"
---
# <a name="the-recoverable-items-folder-is-full"></a>Thư mục mục có thể phục hồi đầy đủ

Đối với hộp thư Exchange Online, giới hạn lưu trữ mặc định cho thư mục mục có thể phục hồi là 30 GB. Giới hạn lưu trữ thư mục mục có thể phục hồi tự động tăng lên 100 GB nếu hộp thư được đặt trên tranh chấp giữ, eDiscovery giữ hoặc được gán cho chính sách lưu giữ.

Khi thư mục mục có thể phục hồi đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo các cách sau:

- Người dùng không thể xoá các mục khỏi hộp thư.

- Hỗ trợ thư mục quản lý không thể xoá các mục dựa trên thẻ lưu giữ hoặc cài đặt thư mục được quản lý.

- Đối với hộp thư có phục hồi một mục kích hoạt hoặc được giữ lại, quá trình sao chép trên viết trang bảo vệ không thể duy trì phiên bản của mục được người dùng biên soạn.

- Đối với hộp thư có hộp kiểm tra đăng nhập kích hoạt, không có mục nhập Nhật ký kiểm tra hộp thư có thể được lưu trong thư mục con kiểm toán trong cặp mục phục hồi.

Đối với hộp thư không tạm giữ, quản trị viên `Search-Mailbox -SearchDumpsterOnly -DeleteContent` có thể sử dụng lệnh trong Exchange Online PowerShell để xoá mục trong thư mục mục có thể phục hồi. Để biết thêm thông tin, hãy xem các chủ đề sau:

- [Tìm kiếm và xóa thư](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Hộp thư tìm kiếm](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Đối với hộp thư đang tạm giữ, quản trị viên phải loại bỏ việc giữ trước khi họ có thể xoá các mục khỏi thư mục mục phục hồi. Để biết thêm thông tin, hãy xem [xóa các mục trong thư mục mục có thể phục hồi của hộp thư dựa trên ứng dụng web qua Internet trên giữ](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Để giúp ngăn không cho thư mục mục có thể phục hồi trở nên đầy đủ, quản trị viên sẽ tăng giới hạn lưu trữ của thư mục mục phục hồi cho hộp thư khi giữ và thiết lập chính sách lưu giữ hộp thư di chuyển các mục từ thư mục mục có thể phục hồi cho hộp thư lưu trữ của người dùng. Xem [tăng dung lượng mục có thể phục hồi cho hộp thư đang giữ](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
