---
title: Triển khai ứng dụng Microsoft 365 dành cho doanh nghiệp để dùng chung trên RDS, Terminal Server hoặc VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200695"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Triển khai ứng dụng Microsoft 365 dành cho doanh nghiệp để dùng chung trên RDS, Terminal Server hoặc VDI

Để triển khai ứng dụng Microsoft 365 cho doanh nghiệp bằng cách dùng dịch vụ Remote trên máy tính (RDS), trước đây có tên là dịch vụ Terminal:

- Bạn phải có gói Microsoft 365 dành cho doanh nghiệp hoặc gói Office 365 bao gồm các ứng dụng Microsoft 365 dành cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.
   > [!NOTE]
   > Các gói Microsoft 365 dành cho doanh nghiệp và Microsoft 365 Business Standard sẽ không bao gồm các ứng dụng Microsoft 365 dành cho doanh nghiệp.
- Bạn phải cho phép [kích hoạt máy tính được chia sẻ](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Bạn cũng có thể tải xuống và chạy công cụ [Trợ giúp phục hồi và hỗ trợ của Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt ứng dụng Microsoft 365 cho doanh nghiệp trong chế độ kích hoạt máy tính dùng chung.

Để biết thêm thông tin về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn về cài đặt tùy chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai ứng dụng Microsoft 365 cho doanh nghiệp bằng cách sử dụng các dịch vụ trên máy tính từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Để khắc phục các lỗi liên quan đến kích hoạt máy tính được chia sẻ:

- Xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Xem [đặt lại ứng dụng Microsoft 365 cho trạng thái kích hoạt doanh nghiệp](https://go.microsoft.com/fwlink/?linkid=2109218).

Nếu bạn muốn cài đặt các ứng dụng Microsoft 365 dành cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng ***thiết đặt cài đặt mặc định***, hãy làm theo các bước sau đây:

1. Kiểm tra xem bạn có đăng ký nào. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Nếu cần, hãy chuyển sang một đăng ký khác. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Nếu Office đã được cài đặt trên máy chủ RDS bằng bất kỳ gói đăng ký nào khác của Microsoft, hãy dỡ cài đặt nó. Ví dụ, bằng cách đi tới **Pa-nen điều khiển** để  >  **gỡ cài đặt một chương trình**. Gỡ cài đặt bằng cách sử dụng trợ [lý phục hồi và hỗ trợ của Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) nếu bạn đang gặp phải vấn đề.
4. Trên máy chủ RDS, hãy đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản người quản trị của bạn và [cài đặt các ứng dụng microsoft 365 cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).
5. Sau khi đã cài đặt Office, ***Đừng mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office nào.
6. Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng cách sửa sổ đăng ký bằng cách thực hiện theo các bước sau đây:
   1. Bấm chuột phải vào nút Windows ở góc dưới bên trái màn hình của bạn, rồi chọn **chạy**. Trong hộp mở, nhập **regedit**, rồi chọn **OK**.
   2. Chọn **có** khi được nhắc để cho phép trình soạn thảo sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.
   3. Trong trình soạn thảo sổ đăng ký, hãy thêm một giá trị chuỗi của **Sharedcomputercấp phép** với một thiết đặt của 1 dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính được chia sẻ được bật cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
