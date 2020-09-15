---
title: Cài đặt Office trên máy chủ kết nối-không được cấp phép
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663139"
---
# <a name="installing-office-on-a-terminal-server"></a>Cài đặt Office trên máy chủ đầu cuối

Đối với triển khai ứng dụng Microsoft 365 cho doanh nghiệp trên Windows Server bằng cách dùng dịch vụ Remote trên máy tính (RDS), trước đây có tên là dịch vụ Terminal:
  
- Bạn phải có đăng ký Microsoft 365 bao gồm các ứng dụng Microsoft 365 cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5. Ứng dụng Microsoft 365 dành cho doanh nghiệp và Microsoft 365 dành cho các gói Business Premium sẽ không bao gồm các ứng dụng Microsoft 365 cho doanh nghiệp.

- Bạn cần cho phép [kích hoạt máy tính được chia sẻ](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Nếu bạn muốn cài đặt các ứng dụng Microsoft 365 cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng các ***thiết đặt cài đặt mặc định***, hãy làm theo các bước sau đây.

> [!TIP]
> Bạn cũng có thể tải xuống và chạy công cụ [Trợ giúp phục hồi và hỗ trợ của Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt ứng dụng Microsoft 365 cho doanh nghiệp trong chế độ kích hoạt máy tính dùng chung.
  
1. Kiểm tra xem bạn có thuê bao Microsoft 365 nào. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Nếu cần, hãy chuyển sang đăng ký khác của Microsoft 365. [Tìm hiểu cách thức](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Nếu Office đã được cài đặt trên máy chủ RDS bằng bất kỳ thuê bao nào khác của Microsoft 365, hãy dỡ cài đặt nó. Ví dụ, bằng cách đi tới Pa-nen điều khiển để \> gỡ cài đặt một chương trình. Gỡ cài đặt bằng cách sử dụng trợ [lý phục hồi và hỗ trợ của Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) nếu bạn đang gặp phải vấn đề.

4. Trên máy chủ RDS, hãy đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản người quản trị của bạn và [cài đặt các ứng dụng microsoft 365 cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).

5. Sau khi đã cài đặt Office, ***Đừng mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office nào.

6. Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng cách sửa sổ đăng ký bằng cách thực hiện theo các bước sau đây:

1. Bấm chuột phải vào nút Windows ở góc dưới bên trái màn hình của bạn, rồi chọn chạy. Trong hộp mở, nhập **regedit**, rồi chọn OK.

2. Chọn có khi được nhắc để cho phép trình soạn thảo sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.

3. Trong trình soạn thảo sổ đăng ký, hãy thêm một giá trị chuỗi của **Sharedcomputercấp phép** với một thiết đặt của 1 dưới HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \ Office\clicktorun\configuration.

7. Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính được chia sẻ được bật cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn về cài đặt tùy chỉnh bằng cách sử dụng công cụ triển khai Office, vui lòng xem [triển khai ứng dụng Microsoft 365 cho doanh nghiệp bằng cách sử dụng các dịch vụ trên máy tính từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Để khắc phục các lỗi liên quan đến kích hoạt máy tính được chia sẻ, vui lòng xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho các ứng dụng Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  