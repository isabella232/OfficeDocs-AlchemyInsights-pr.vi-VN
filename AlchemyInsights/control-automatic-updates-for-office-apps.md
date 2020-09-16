---
title: Điều khiển Cập nhật tự động cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747798"
---
# <a name="control-automatic-updates-for-office-apps"></a>Điều khiển Cập nhật tự động cho các ứng dụng Office

Theo mặc định, các bản Cập Nhật cho các ứng dụng Office được tự động tải xuống và áp dụng trong nền mà không có bất kỳ sự can thiệp của người dùng. Tuy nhiên, người quản trị có thể kiểm soát cách áp dụng các bản Cập Nhật bằng cách dùng thiết đặt Cập Nhật Office. Thiết đặt Cập Nhật cho phép người quản trị bật hoặc tắt Cập nhật tự động, Hiển thị hoặc ẩn nút **Cập Nhật ngay** trong Office, đặt thời hạn Cập Nhật và nhiều hơn nữa. Để biết thông tin chi tiết, hãy xem:

- [Cấu hình thiết đặt Cập Nhật cho Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Cập nhật tự động cho Office không được bật](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Xác định cách Cập Nhật Office sau khi cài đặt nó](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Để xem lại các thiết đặt Cập Nhật hiện có được áp dụng cho máy khách, hãy làm theo các bước sau:

1. Mở trình soạn thảo sổ đăng ký bằng cách đi đến **bắt đầu**  >  **chạy**  >  **regedit**.
2. Chuyển đến vị trí sau đây và xem lại các thiết đặt Cập Nhật Office:  
    một. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. Gỡ cài đặt cấu hình

**Ghi chú**  Nếu khóa officemgmtcom được đặt, bạn có thể thấy thông báo "bản Cập Nhật được quản lý bởi người quản **Office**trị hệ thống của bạn" trong các  >  **Account**  >  **bản Cập Nhật**tài khoản Office. Để biết thêm thông tin, hãy xem [quản lý các bản Cập Nhật cho ứng dụng microsoft 365 với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  