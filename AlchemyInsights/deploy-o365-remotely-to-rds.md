---
title: Triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp để sử dụng chung trên RDS, Terminal Server hoặc VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507608"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp để sử dụng chung trên RDS, Terminal Server hoặc VDI

Triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:
- Bạn phải có Microsoft 365 cho kế hoạch kinh doanh hoặc gói Office 365 bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 ứng dụng dành cho doanh nghiệp và Microsoft 365 Business Premium Standard gói không bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp.
- Bạn phải kích [hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Microsoft 365 Apps dành cho doanh nghiệp ở chế độ kích hoạt máy tính dùng chung.

Để biết thêm thông tin về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung:
- Xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Xem [đặt lại Microsoft 365 ứng dụng cho trạng thái kích hoạt doanh nghiệp](https://go.microsoft.com/fwlink/?linkid=2109218).

Nếu bạn muốn cài đặt Microsoft 365 Apps dành cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng ***cài đặt mặc định***, sử dụng các bước sau:

1.    Kiểm tra những gì bạn có đăng ký. [Tìm hiểu làm thế nào](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Nếu cần thiết, chuyển sang đăng ký khác. [Tìm hiểu làm thế nào](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Nếu Office đã được cài đặt trên máy chủ RDS bằng bất kỳ gói đăng ký Microsoft nào khác, hãy gỡ cài đặt. Ví dụ, bằng cách đi tới **bảng điều khiển**  >  **gỡ bỏ cài đặt một chương trình**. Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.
4.    Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt microsoft 365 Apps dành cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).
5.    Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.
6.    Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:
   1. Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn **chạy**. Trong ô mở, gõ **regedit**, và sau đó chọn **OK**.
   2. Chọn **có** khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.
   3. Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Trên máy chủ RDS, ***đăng nhập như người dùng cuối*** và [xác minh rằng kích hoạt chia sẻ máy tính được kích hoạt cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

