---
title: Khắc phục sự OneDrive cố
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921029"
---
# <a name="troubleshoot-onedrive-crashes"></a>Khắc phục sự OneDrive cố

Nếu bạn OneDrive liên tục gặp sự cố, hãy thử các bước khắc phục sự cố sau:

**Đảm bảo khóa đăng ký không được đặt:**

1. Sử dụng Trình soạn thảo Sổ đăng ký, dẫn hướng HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Nếu DisableFileSyncNGSC hiện diện và đặt là 1, hãy mở khóa và thay đổi giá trị thành 0.
3. Khởi chạy thủ OneDrive bằng cách đi tới Bắt đầu ![Nhấn phím Windows phải](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.

**Đặt lại OneDrive:**

Lưu ý:

- Việc đặt lại OneDrive kết nối tất cả các kết nối đồng bộ hiện có của bạn (bao gồm kết nối OneDrive cá nhân của bạn nếu được thiết lập).
- Bạn sẽ không bị mất tệp hay dữ liệu khi đặt lại OneDrive máy tính của mình.

**Cách đặt lại OneDrive:**

1. Mở hộp thoại Chạy bằng cách Windows phím Windows và R.
2. Nhập %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, rồi nhấn OK. Cửa sổ Lệnh có thể xuất hiện trong thời gian ngắn.
3. Khởi chạy thủ OneDrive bằng cách đi tới Bắt đầu ![Nhấn phím Windows phải](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.

Lưu ý:

- Nếu bạn đã chọn chỉ đồng bộ một số thư mục trước khi đặt lại, bạn sẽ cần thực hiện lại điều đó sau khi đồng bộ xong. Đọc [mục Chọn thư OneDrive mục cần đồng bộ với máy tính của bạn để](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)biết thêm thông   tin.
- Bạn sẽ cần hoàn tất việc này cho tài khoản cá nhân OneDrive và OneDrive for Business.