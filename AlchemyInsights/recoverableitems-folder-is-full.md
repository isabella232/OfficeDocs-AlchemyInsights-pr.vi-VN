---
title: thư mục 1336 RecoverableItems đã đầy
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741289"
---
# <a name="the-recoverable-items-folder-is-full"></a>Thư mục các mục có thể phục hồi được đầy đủ

Đối với hộp thư Exchange Online, giới hạn dung lượng lưu trữ mặc định cho thư mục các mục có thể phục hồi là 30 GB. Giới hạn lưu trữ cho thư mục các mục có thể phục hồi được tự động tăng lên 100 GB nếu hộp thư được đặt ở chế độ duy trì tranh chấp, hãy giữ khám phá điện tử hoặc được gán cho chính sách duy trì.

Khi thư mục các mục có thể phục hồi đạt đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo những cách sau đây:

- Người dùng không thể xóa bỏ các mục khỏi hộp thư.

- Trợ lý thư mục được quản lý không thể xóa các mục dựa trên thẻ lưu giữ hoặc thiết đặt thư mục được quản lý.

- Đối với các hộp thư có kích hoạt mục duy nhất được bật hoặc được đặt ở chế độ chờ, quy trình bảo vệ bản sao trên trang không thể duy trì các phiên bản của các mục do người dùng chỉnh sửa.

- Đối với hộp thư có bật ghi nhật ký kiểm tra hộp thư, không có mục nhập Nhật ký kiểm tra hộp thư nào có thể được lưu trong thư mục con trong thư mục các mục có thể phục hồi.

Đối với hộp thư không ở trạng thái giữ, người quản trị có thể sử dụng `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lệnh trong Exchange Online PowerShell để xóa các mục trong thư mục các mục có thể phục hồi. Để biết thêm thông tin, hãy xem các chủ đề sau:

- [Tìm kiếm và xóa thư](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Tìm kiếm-hộp thư](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Đối với hộp thư đang ở trạng thái giữ, người quản trị phải loại bỏ giữ trước khi họ có thể xóa các mục khỏi thư mục các mục có thể phục hồi. Để biết thêm thông tin, hãy xem [mục xóa mục trong thư mục các mục có thể phục hồi của các hộp thư trên nền tảng điện toán đám mây](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Để ngăn không cho thư mục các mục có thể phục hồi trở nên đầy đủ, người quản trị có thể tăng giới hạn lưu trữ của thư mục các mục có thể phục hồi cho hộp thư khi giữ và thiết lập chính sách duy trì hộp thư di chuyển các mục từ thư mục các mục có thể phục hồi tới hộp thư lưu trữ của người dùng. Hãy xem [mục tăng hạn ngạch các mục có thể phục hồi cho hộp thư ở](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)chế độ chờ.
