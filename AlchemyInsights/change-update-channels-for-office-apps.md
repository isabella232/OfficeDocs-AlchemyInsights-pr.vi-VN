---
title: Thay đổi các kênh Cập Nhật cho các ứng dụng Office
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
ms.openlocfilehash: fb69bce40ab56b162c715af6a0647c8219c5564f
ms.sourcegitcommit: dab885f2cb99057e959fb9be334f5a3a26a64058
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46665484"
---
# <a name="change-update-channels-for-office-apps"></a>Thay đổi các kênh Cập Nhật cho các ứng dụng Office

Đối với các bản cài đặt Office mới, hãy dùng thiết đặt tải xuống phần mềm Office để chọn kênh Cập Nhật mong muốn, sau đó cài đặt (hoặc cài đặt lại) các ứng dụng Office. Để biết thêm thông tin, hãy xem [quản lý các thiết đặt tải xuống phần mềm trong Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Ghi chú** Kênh Cập Nhật được chọn bằng cách sử dụng thiết đặt tải xuống phần mềm Office áp dụng cho tất cả người dùng thực hiện cài đặt mới bằng cách dùng cổng thông tin O365. Để biết thêm thông tin, hãy xem [tải xuống và cài đặt hoặc cài đặt lại Microsoft 365 hoặc Office 2019 trên PC hoặc máy Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Đối với các bản cài đặt Office hiện có, hãy sử dụng công cụ triển khai Office (ODT) để chuyển sang kênh Cập Nhật khác:  

1. Tải xuống phiên bản mới nhất của công cụ triển khai Office (setup.exe) từ [Trung tâm tải xuống của Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Xác định tên kênh mà bạn muốn chuyển sang. Để biết thêm thông tin, hãy xem [tùy chọn cấu hình cho công cụ triển khai Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Tạo một tệp XML cấu hình xác định tên kênh thích hợp, ví dụ, update.xml.  
    `<Configuration> 
    <Updates **Channel="Monthly"** />  
    </Configuration>`
4. Từ dấu nhắc lệnh nâng cao, hãy chuyển đến vị trí thư mục nơi setup.exe cư trú và chạy lệnh sau đây:  
    một. setup.exe/Configure update.xml
5. Khởi động một ứng dụng Office (chẳng hạn như Excel), **File**rồi chọn  >  **tài khoản**tệp. Trong phần thông tin sản phẩm, chọn Cập Nhật **tùy chọn cập**Nhật  >  **ngay bây giờ**.

Để biết thêm thông tin, hãy xem [làm thế nào để chuyển các kênh Cập Nhật cho các ứng dụng Office hiện có](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Để chuyển đổi các kênh Cập Nhật cho một nhóm người dùng được chọn hoặc bằng cách sử dụng trình quản lý cấu hình (SCCM), cấu hình thiết đặt kênh Cập Nhật bằng GPO. Để biết thêm thông tin, hãy xem [tổng quan về các kênh Cập Nhật cho ứng dụng Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Để biết chi tiết, hãy xem [làm thế nào để quản lý các kênh Office 365 ProPlus cho CNTT ưu](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) và [quản lý các bản Cập Nhật cho ứng dụng Microsoft 365 với Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).