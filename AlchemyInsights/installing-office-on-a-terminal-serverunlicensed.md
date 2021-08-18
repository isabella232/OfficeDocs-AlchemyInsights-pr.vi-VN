---
title: Cài đặt office trên Terminal Server - Chưa được cấp phép
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322021"
---
# <a name="installing-office-on-a-terminal-server"></a>Cài Office trên Máy chủ Đầu cuối

Để triển khai Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn trên một Máy chủ Windows dùng Dịch vụ Máy tính Từ xa (RDS), trước đây có tên là Dịch vụ Thiết bị Đầu cuối:
  
- Bạn phải có đăng ký Microsoft 365 bao gồm Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn như Office 365 Enterprise E3 hoặc Enterprise E5. Gói Ứng dụng Microsoft 365 dành cho doanh nghiệp và Ứng dụng Microsoft 365 dành cho doanh nghiệp Premium không bao gồm các bản Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.

- Bạn cần cho phép kích [hoạt máy tính dùng chung.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Nếu bạn muốn cài đặt Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn RDS từ trung Trung tâm quản trị Microsoft 365 sử dụng cài đặt ***mặc*** định , hãy sử dụng các bước sau đây.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Kiểm tra xem Microsoft 365 ký nào bạn có. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Nếu cần, hãy chuyển sang đăng ký Microsoft 365 khác. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Nếu máy Office đã được cài đặt trên máy chủ RDS bằng bất kỳ đăng ký Microsoft 365 nào khác, hãy gỡ cài đặt nó. Ví dụ: bằng cách đi tới Gỡ cài đặt một chương trình trong Panel \> Điều khiển. Gỡ cài [đặt bằng cách sử Công cụ Trợ giúp Phục hồi và Hỗ trợ](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft nếu bạn đang gặp sự cố.

4. Trên máy chủ RDS, đăng nhập vào trang web bằng Trung tâm quản trị Microsoft 365 quản trị viên của bạn và [cài đặt Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://portal.office.com/OLS/MySoftware.aspx)

5. Sau Office được cài đặt, ***đừng mở hoặc đăng nhập vào bất kỳ ứng*** dụng Office nào.

6. Trên máy chủ RDS, bật kích hoạt máy tính dùng chung bằng cách chỉnh sửa sổ đăng ký bằng cách làm theo các bước sau:

1. Bấm chuột phải vào Windows Màn hình ở góc dưới bên trái màn hình, rồi chọn Chạy. Trong hộp Mở, nhập **regedit**, rồi chọn OK.

2. Chọn Có khi được nhắc cho phép Trình soạn thảo Sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.

3. Trong Trình soạn thảo Sổ đăng ký, thêm giá trị chuỗi **của SharedComputerLicensing** với cài đặt là 1 bên dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Trên máy chủ RDS, đăng nhập với ***tư cách người*** dùng cuối và xác minh rằng kích hoạt máy tính dùng chung đã được kích hoạt [Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Để biết thêm chi tiết về các điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn về các cài đặt tùy chỉnh bằng cách sử dụng Công cụ Triển khai Office, vui lòng xem Triển khai [Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)bằng cách sử dụng Dịch vụ Máy tính Từ xa .
  
Để khắc phục các lỗi liên quan đến việc kích hoạt máy tính dùng chung, vui lòng [xem Khắc phục sự cố với việc kích hoạt máy tính Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  