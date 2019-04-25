---
title: 1336 RecoverableItems thư mục là đầy đủ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389105"
---
# <a name="the-recoverable-items-folder-is-full"></a>Thư mục mục có thể phục hồi được đầy đủ

Đối với hộp thư Exchange Online trong Office 365, giới hạn dung lượng mặc định cho thư mục mục có thể phục hồi là 30 GB. Giới hạn lưu trữ cho thư mục mục có thể phục hồi tự động tăng lên tới 100 GB nếu hộp thư được đặt trên tranh chấp giữ, Giữ lại eDiscovery, hoặc được gán cho một chính sách lưu giữ Office 365.

Khi thư mục mục có thể phục hồi đạt đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo các cách sau:

- Người dùng không thể xoá các mục khỏi hộp thư.

- Chương trình hỗ trợ thư mục quản lý không thể xoá các mục dựa trên thẻ lưu giữ hoặc cài đặt thư mục được quản lý.

- Cho hộp thư đã khôi phục từng mục duy nhất kích hoạt hoặc được đặt trên giữ, quá trình bảo vệ bản sao trên viết trang không thể duy trì các phiên bản của bài chỉnh sửa của người dùng.

- Cho các hộp thư có hộp thư được kích hoạt ghi nhật ký kiểm tra, không có mục nào đăng nhập hộp thư kiểm tra có thể được lưu trong thư mục kiểm tra trong thư mục mục có thể phục hồi.

Hộp thư không phải là tổ chức, quản trị viên có thể sử dụng các `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lệnh trong Exchange Online PowerShell để xóa các khoản mục trong thư mục mục có thể phục hồi. Để biết thêm thông tin, hãy xem các chủ đề sau: 

- [Tìm kiếm và xoá thư](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Hộp thư tìm kiếm](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Cho các hộp thư về tổ chức, quản trị viên có để loại bỏ các giữ trước khi họ có thể các khoản mục đã xóa khỏi thư mục mục có thể phục hồi. Để biết thêm chi tiết, hãy xem [xóa các khoản mục trong các mục có thể phục hồi các thư mục trong hộp thư dựa trên giữ](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Để giúp ngăn ngừa thư mục mục có thể phục hồi từ trở nên đầy đủ, quản trị viên có thể tăng giới hạn lưu trữ các mục có thể phục hồi các thư mục hộp thư vào tổ chức và thiết lập một chính sách lưu giữ hộp thư di chuyển khoản mục khỏi thư mục mục có thể phục hồi để lưu trữ của người dùng hộp thư. Thấy [tăng các khoản mục có thể phục hồi định mức cho hộp thư trên tổ chức](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
