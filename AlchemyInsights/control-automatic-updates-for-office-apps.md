---
title: Điều khiển tự động cập nhật cho Office Apps
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
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929903"
---
# <a name="control-automatic-updates-for-office-apps"></a>Điều khiển tự động cập nhật cho Office Apps

Theo mặc định, các bản cập nhật cho Office ứng dụng được tải xuống tự động và áp dụng trong nền mà không cần sự can thiệp của người dùng. Tuy nhiên, người quản trị có thể kiểm soát cách áp dụng các bản cập nhật bằng cách Office đặt Update. Thiết đặt cập nhật cho phép người quản  trị bật hoặc tắt cập nhật tự động, hiển thị hoặc ẩn nút Cập nhật Ngay trong thiết Office, đặt hạn chót cập nhật và nhiều hơn nữa. Để biết thông tin chi tiết, hãy xem:

- [Cấu hình thiết đặt cập nhật cho Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Tính năng tự động cập Office cập nhật không được bật](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Xác định cách Office cập nhật sau khi cài đặt](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Để xem lại các cài đặt bản cập nhật hiện có được áp dụng cho máy khách, hãy làm theo các bước sau:

1. Mở Trình soạn thảo Sổ đăng ký bằng cách đi **tới Bắt đầu**  >  **Chạy**  >  **regedit.**
2. Chuyển đến vị trí sau đây và xem lại thiết Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Lưu ý**  Nếu khóa OfficeMgmtCOM được đặt, bạn có thể thấy thông báo "Các bản cập nhật được quản lý bởi người quản trị hệ thống của bạn" trong Office cập nhật  >    >  **tài Office của bạn.** Để biết thêm thông tin, hãy [xem mục Quản lý các bản cập nhật Ứng dụng Microsoft 365 với Microsoft Endpoint Configuration Manager.](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)  