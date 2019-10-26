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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205431"
---
# <a name="installing-office-on-a-terminal-server"></a>Cài đặt Office trên máy chủ đầu cuối

Để triển khai Office 365 ProPlus trên Windows Server sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:
  
- Bạn phải có một gói Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5. Các gói Office 365 Business và Office 365 Business Premium không bao gồm Office 365 ProPlus.

- Bạn cần bật [kích hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ Trung tâm quản trị Microsoft 365, sử ***dụng cài đặt mặc định***, sử dụng các bước sau.

> [!TIP]
> Bạn cũng có thể tải xuống và chạy [Microsoft support và Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) để cài đặt Office 365 ProPlus trong chế độ kích hoạt máy tính dùng chung.
  
1. Kiểm tra những gì Office 365 kế hoạch bạn có. [Tìm hiểu cách](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Nếu cần thiết, chuyển sang một gói Office 365 khác. [Tìm hiểu cách](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch Office 365 khác, dỡ cài đặt. Ví dụ: bằng cách đi tới Pa \> -nen điều khiển gỡ cài đặt chương trình. Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.

4. Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.

6. Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:

1. Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn chạy. Trong ô mở, gõ **regedit**, và sau đó chọn OK.

2. Chọn có khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.

3. Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính dùng chung được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung, vui lòng xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  