---
title: Khắc phục sự cố OneDrive sập
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749243"
---
# <a name="troubleshoot-onedrive-crashes"></a>Khắc phục sự cố OneDrive sập

Nếu OneDrive liên tục sập, hãy thử các bước khắc phục sự cố sau:

**Đảm bảo khoá đăng ký không thiết lập:**

1. Sử dụng Registry Editor, điều hướng đến HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Nếu DisableFileSyncNGSC có và đặt thành 1, mở khoá và thay đổi giá trị thành 0.
3. Khởi chạy bằng tay OneDrive bằng cách đi tới bắt đầu ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm rồi bấm vào ứng dụng OneDrive dành cho máy tính để bàn.

**Đặt lại OneDrive:**

Ghi chú:

- Việc đặt lại OneDrive ngắt kết nối tất cả các kết nối đồng bộ hiện có của bạn (bao gồm OneDrive cá nhân của bạn nếu thiết lập).
- Bạn sẽ không mất tệp hoặc dữ liệu bằng việc đặt lại OneDrive trên máy tính của mình.

**Để đặt lại OneDrive:**

1. Mở hộp thoại chạy bằng cách nhấn phím Windows và R.
2. Nhập% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset và nhấn OK. Một cửa sổ lệnh có thể xuất hiện một thời gian ngắn.
3. Khởi chạy bằng tay OneDrive bằng cách đi tới bắt đầu ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm rồi bấm vào ứng dụng OneDrive dành cho máy tính để bàn.

Ghi chú:

- Nếu bạn đã chọn để đồng bộ chỉ một số thư mục trước khi đặt lại, bạn sẽ cần phải làm điều đó một lần nữa đồng bộ đã hoàn thành. Đọc [chọn thư mục OneDrive để đồng bộ hóa với máy tính của bạn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)để biết   thêm thông tin.
- Bạn sẽ cần hoàn tất việc này cho OneDrive và OneDrive dành cho doanh nghiệp cá nhân của mình.