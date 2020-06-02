---
title: Cài đặt Office trên máy chủ đầu cuối-không có giấy phép
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508650"
---
# <a name="installing-office-on-a-terminal-server"></a>Cài đặt Office trên máy chủ đầu cuối

Để triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp trên Windows Server sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:
  
- Bạn phải đăng ký Microsoft 365 bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5. Các ứng dụng Microsoft 365 dành cho doanh nghiệp và Microsoft 365 ứng dụng dành cho doanh nghiệp Premium gói không bao gồm Microsoft 365 ứng dụng dành cho doanh nghiệp.

- Bạn cần bật [kích hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Nếu bạn muốn cài đặt Microsoft 365 Apps dành cho doanh nghiệp trên RDS từ Trung tâm quản trị Microsoft 365, sử dụng ***cài đặt mặc định***, sử dụng các bước sau.

> [!TIP]
> Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Microsoft 365 Apps dành cho doanh nghiệp ở chế độ kích hoạt máy tính dùng chung.
  
1. Kiểm tra những gì Microsoft 365 đăng ký bạn có. [Tìm hiểu cách](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Nếu cần, chuyển sang đăng ký Microsoft 365 khác. [Tìm hiểu cách](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ đăng ký Microsoft 365 khác, dỡ cài đặt. Ví dụ: bằng cách đi tới Pa-nen điều khiển \> gỡ cài đặt chương trình. Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.

4. Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt microsoft 365 Apps dành cho doanh nghiệp](https://portal.office.com/OLS/MySoftware.aspx).

5. Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.

6. Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:

1. Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn chạy. Trong ô mở, gõ **regedit**, và sau đó chọn OK.

2. Chọn có khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.

3. Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Trên máy chủ RDS, ***đăng nhập như người dùng cuối*** và [xác minh rằng kích hoạt chia sẻ máy tính được kích hoạt cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Microsoft 365 ứng dụng dành cho doanh nghiệp bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung, hãy xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Microsoft 365 ứng dụng dành cho doanh nghiệp](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  