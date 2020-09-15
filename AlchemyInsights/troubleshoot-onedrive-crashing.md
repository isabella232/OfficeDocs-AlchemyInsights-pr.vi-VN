---
title: Khắc phục sự cố OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665020"
---
# <a name="troubleshoot-onedrive-crashes"></a>Khắc phục sự cố OneDrive

Nếu OneDrive liên tục gặp sự cố, hãy thử các bước khắc phục sự cố sau:

**Đảm bảo các phím registry không được đặt:**

1. Sử dụng trình soạn thảo sổ đăng ký, dẫn hướng đến HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Nếu giải pháp thay thế là trình bày và đặt thành 1, hãy mở khóa và thay đổi giá trị thành 0.
3. Khởi động OneDrive theo cách thủ công bằng cách đi đến bắt đầu ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.

**Đặt lại OneDrive:**

Boy

- Việc đặt lại OneDrive đã ngắt kết nối tất cả các kết nối đồng bộ hiện có của bạn (bao gồm OneDrive cá nhân của bạn nếu thiết lập).
- Bạn sẽ không mất tệp hoặc dữ liệu bằng cách đặt lại OneDrive trên máy tính của mình.

**Để đặt lại OneDrive:**

1. Mở hộp thoại chạy bằng cách nhấn phím Windows và R.
2. Nhập% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset và nhấn OK. Một cửa sổ lệnh có thể xuất hiện một thời gian ngắn.
3. Khởi động OneDrive theo cách thủ công bằng cách đi đến bắt đầu ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.

Boy

- Nếu bạn đã chọn chỉ đồng bộ một số thư mục trước khi đặt lại, bạn sẽ cần thực hiện lại sau khi đồng bộ đã hoàn thành. Đọc [chọn thư mục OneDrive để đồng bộ với máy tính của bạn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)để   biết thêm thông tin.
- Bạn sẽ cần hoàn thành đối với OneDrive và OneDrive for Business của bạn.