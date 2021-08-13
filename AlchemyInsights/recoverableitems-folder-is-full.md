---
title: 1336 Thư mục Mục Có thể phục hồi đã đầy
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061778"
---
# <a name="the-recoverable-items-folder-is-full"></a>Thư mục Các mục Có thể phục hồi đã đầy

Đối với Exchange Online thư, giới hạn lưu trữ mặc định cho thư mục Các mục Có thể phục hồi là 30 GB. Giới hạn lưu trữ cho thư mục Các mục Có thể phục hồi được tự động tăng lên đến 100 GB nếu hộp thư được đặt ở chế độ Bảo quản thư trong Trường hợp tranh chấp, giữ Khám phá Điện tử hoặc được gán cho chính sách duy trì.

Khi thư mục Các mục Có thể phục hồi đạt đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo những cách sau đây:

- Người dùng không thể xóa các mục khỏi hộp thư.

- Trợ lý Thư mục có Quản lý không thể xóa các mục dựa trên thẻ duy trì hoặc thiết đặt thư mục được quản lý.

- Đối với hộp thư có bật hoặc giữ Lại Mục Đơn, quy trình bảo vệ trang sao chép vào ghi không thể duy trì phiên bản các mục đã chỉnh sửa của người dùng.

- Đối với các hộp thư đã bật tính năng ghi nhật ký kiểm tra hộp thư, bạn không thể lưu các mục nhật ký kiểm tra hộp thư vào thư mục con Kiểm tra trong thư mục Các mục Có thể phục hồi.

Đối với những hộp thư không được lưu giữ, người quản trị có thể sử dụng lệnh trong PowerShell Exchange Online để xóa các mục trong thư mục `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Các mục Có thể phục hồi. Để biết thêm thông tin, hãy xem các chủ đề sau:

- [Tìm kiếm và xóa thư](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Đối với hộp thư đang chờ, người quản trị phải loại bỏ giữ trước khi có thể xóa các mục khỏi thư mục Các mục Có thể khôi phục. Để biết thêm thông tin, hãy [xem mục Xóa mục trong thư mục Các mục Có thể phục hồi của hộp](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)thư trên nền điện toán đám mây đang chờ .

Để giúp ngăn thư mục Các mục Có thể phục hồi trở thành đầy đủ, người quản trị có thể tăng giới hạn lưu trữ của thư mục Các mục Có thể phục hồi cho hộp thư bị giữ và thiết lập chính sách duy trì hộp thư giúp di chuyển các mục từ thư mục Các mục Có thể phục hồi đến hộp thư lưu trữ của người dùng. Xem [mục Tăng hạn mức Các mục Có thể phục hồi cho các hộp thư tạm cầm .](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
