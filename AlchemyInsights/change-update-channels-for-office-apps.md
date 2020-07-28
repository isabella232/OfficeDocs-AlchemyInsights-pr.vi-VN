---
title: Thay đổi kênh Cập Nhật cho các ứng dụng Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440026"
---
# <a name="change-update-channels-for-office-apps"></a>Thay đổi kênh Cập Nhật cho các ứng dụng Office

Để cài đặt Office mới, sử dụng cài đặt tải xuống phần mềm Office để chọn kênh Cập Nhật mong muốn, và sau đó cài đặt (hoặc cài đặt lại) ứng dụng Office. Để biết thêm thông tin, xem [quản lý cài đặt tải xuống phần mềm trong Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Lưu ý** Kênh Cập Nhật được chọn bằng cách sử dụng cài đặt tải xuống phần mềm Office áp dụng cho tất cả người dùng thực hiện cài đặt mới bằng cách sử dụng cổng thông tin O365. Để biết thêm thông tin, xem [tải xuống và cài đặt hoặc cài đặt lại Microsoft 365 hoặc Office 2019 trên PC hoặc máy Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Để cài đặt Office hiện tại, sử dụng công cụ triển khai Office (ODT) để chuyển sang một kênh Cập Nhật khác:  

1. Tải xuống phiên bản mới nhất của công cụ triển khai Office (setup.exe) từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Xác định tên của kênh mà bạn muốn chuyển sang. Để biết thêm thông tin, hãy xem [tùy chọn cấu hình cho công cụ triển khai Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Tạo một tệp XML cấu hình xác định tên kênh phù hợp, ví dụ: update.xml.  
    A. <Configuration>  
    B. <Cập Nhật **Channel = "hàng tháng"** />  
    C. </Configuration>
4. Từ dấu nhắc lệnh nâng cao, chuyển sang vị trí thư mục nơi setup.exe cư trú và chạy lệnh sau:  
    A. setup.exe/cấu hình update.xml
5. Khởi động ứng dụng Office (chẳng hạn như Excel), và **File**sau đó chọn  >  **tài khoản**tệp. Trong phần thông tin sản phẩm, chọn **Cập nhật tùy chọn Update**  >  **ngay bây giờ**.

Để biết thêm thông tin, xem [cách chuyển đổi kênh Cập Nhật cho các ứng dụng Office hiện có](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Để chuyển đổi kênh Cập Nhật cho một nhóm người dùng được chọn hoặc bằng cách sử dụng trình quản lý cấu hình (SCCM), cấu hình cài đặt kênh Cập Nhật bằng cách sử dụng GPO. Để biết thêm thông tin, xem [tổng quan về các kênh Cập Nhật cho Microsoft 365 ứng dụng](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Để biết chi tiết, xem [cách quản lý các kênh Office 365 ProPlus dành cho chuyên gia CNTT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) và [quản lý các bản cập nhật cho Microsoft 365 Apps với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).