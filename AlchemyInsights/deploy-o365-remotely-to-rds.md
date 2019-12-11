---
title: Triển khai Office 365 ProPlus để sử dụng chung trên RDS, Terminal Server, hoặc VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959481"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Triển khai Office 365 ProPlus để sử dụng chung trên RDS, Terminal Server, hoặc VDI

Triển khai Office 365 ProPlus sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên là dịch vụ đầu cuối:
- Bạn phải có Microsoft 365 cho kế hoạch kinh doanh hoặc gói Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.
   > [!NOTE] 
   > Các gói Office 365 Business và Office 365 Business Premium không bao gồm Office 365 ProPlus.
- Bạn phải kích [hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Office 365 ProPlus trong chế độ kích hoạt máy tính dùng chung.

Để biết thêm thông tin về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung:
- Xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Xem [đặt lại trạng thái kích hoạt Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ Trung tâm quản trị Microsoft 365, sử ***dụng cài đặt mặc định***, sử dụng các bước sau:

1.  Kiểm tra những gì Office 365 kế hoạch bạn có. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Nếu cần thiết, chuyển sang một gói Office 365 khác. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch Office 365 khác, dỡ cài đặt. Ví dụ, bằng cách đi tới >  **bảng điều khiển****gỡ bỏ cài đặt một chương trình**. Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.
4.  Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.
6.  Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:
   1. Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn **chạy**. Trong ô mở, gõ **regedit**, và sau đó chọn **OK**.
   2. Chọn **có** khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.
   3. Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính dùng chung được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

