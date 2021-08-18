---
title: Triển khai Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn dùng chung trên RDS, Máy chủ Đầu cuối hoặc VDI
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325625"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Triển khai Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn dùng chung trên RDS, Máy chủ Đầu cuối hoặc VDI

Để triển khai các Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn dùng Dịch vụ Máy tính Từ xa (RDS), trước đây gọi là Dịch vụ Thiết bị Đầu cuối:

- Bạn phải có một Microsoft 365 dành cho Doanh nghiệp hoặc một gói Office 365 bao gồm Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.
   **Lưu** ý : Các Ứng dụng Microsoft 365 dành cho doanh nghiệp và Microsoft 365 Business Standard không bao gồm các Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.
- Bạn phải cho phép kích [hoạt máy tính dùng chung.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Lưu** ý : Bạn cũng có thể tải xuống và chạy [Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ](https://aka.ms/SaRA_OfficeSCA_M365Portal) cài đặt Máy tính Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn chế độ kích hoạt máy tính dùng chung.

Để biết thêm thông tin về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn về các cài đặt tùy chỉnh bằng cách sử dụng Công cụ Triển khai Office, hãy xem Triển khai [Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)bằng cách sử dụng Dịch vụ Máy tính Từ xa.

Để khắc phục các lỗi liên quan đến việc kích hoạt máy tính dùng chung:

- Xem khắc [phục sự cố với kích hoạt máy tính dùng chung Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Hãy xem [Đặt lại Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn thái kích hoạt](https://go.microsoft.com/fwlink/?linkid=2109218).

Nếu bạn muốn cài đặt Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn RDS từ Trung Trung tâm quản trị Microsoft 365 sử dụng cài đặt ***mặc*** định , hãy sử dụng các bước sau đây:

1. Kiểm tra xem bạn có đăng ký nào. [Tìm hiểu cách thực hiện](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Nếu cần, hãy chuyển sang đăng ký khác. [Tìm hiểu cách thực hiện](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Nếu máy Office đã được cài đặt trên máy chủ RDS bằng cách sử dụng bất kỳ đăng ký Microsoft nào khác, hãy gỡ cài đặt nó. Ví dụ: bằng cách đi tới Gỡ **cài đặt chương trình trong Panel** Điều  >  **khiển**. Gỡ cài [đặt bằng cách sử Công cụ Trợ giúp Phục hồi và Hỗ trợ](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft nếu bạn đang gặp sự cố.
4. Trên máy chủ RDS, đăng nhập vào trang web bằng Trung tâm quản trị Microsoft 365 quản trị viên của bạn và [cài đặt Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://portal.office.com/OLS/MySoftware.aspx)
5. Sau Office được cài đặt, ***đừng mở hoặc đăng nhập vào bất kỳ ứng*** dụng Office nào.
6. Trên máy chủ RDS, bật kích hoạt máy tính dùng chung bằng cách chỉnh sửa sổ đăng ký bằng cách làm theo các bước sau:
   1. Bấm chuột phải vào Windows màn hình ở góc dưới bên trái màn hình, rồi chọn **Chạy**. Trong hộp Mở, nhập **regedit**, sau đó chọn **OK**.
   2. Chọn **Có khi** được nhắc cho phép Trình soạn thảo Sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.
   3. Trong Trình soạn thảo Sổ đăng ký, thêm giá trị chuỗi **của SharedComputerLicensing** với thiết đặt 1 dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Trên máy chủ RDS, đăng nhập với ***tư cách người*** dùng cuối và xác minh rằng kích hoạt máy tính dùng chung đã được bật cho người [Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
