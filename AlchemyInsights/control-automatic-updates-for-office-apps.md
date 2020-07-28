---
title: Kiểm soát Cập nhật tự động cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439930"
---
# <a name="control-automatic-updates-for-office-apps"></a>Kiểm soát Cập nhật tự động cho các ứng dụng Office

Theo mặc định, bản Cập Nhật cho ứng dụng Office được tải xuống tự động và áp dụng trong nền mà không cần bất kỳ sự can thiệp của người dùng. Tuy nhiên, quản trị viên có thể kiểm soát cách áp dụng bản Cập Nhật bằng cách sử dụng cài đặt Office Update. Cài đặt Cập Nhật cho phép quản trị viên bật hoặc tắt Cập nhật tự động, Hiển thị hoặc ẩn nút **Cập Nhật ngay** trong Office, đặt Cập Nhật thời hạn và hơn thế nữa. Để biết thông tin chi tiết, xem:

- [Cấu hình cài đặt bản Cập Nhật cho Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Cập nhật tự động cho Office không được kích hoạt](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Xác định cách Office được cập nhật sau khi cài đặt](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Để đánh giá cài đặt bản Cập Nhật hiện tại được áp dụng cho máy khách, hãy làm theo các bước sau:

1. Mở Registry Editor bằng đi để **bắt đầu**  >  **chạy**  >  **regedit**.
2. Chuyển sang vị trí sau và đánh giá cài đặt Cập Nhật Office:  
    A. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    B. ClickToRun\Configuration

**Lưu ý**  Nếu khoá officemgmtcom được thiết lập, bạn có thể thấy thông báo "Cập Nhật được quản lý bởi quản trị hệ thống của bạn **" trong văn phòng**  >  **tài khoản**Office  >  **Cập Nhật**. Để biết thêm thông tin, xem [quản lý bản Cập Nhật cho microsoft 365 ứng dụng với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  