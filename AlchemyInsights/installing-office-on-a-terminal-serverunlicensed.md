---
title: Cài đặt office trên một máy chủ đầu cuối - không có giấy phép
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29497067"
---
# <a name="installing-office-on-a-terminal-server"></a>Cài đặt Office trên một máy chủ đầu cuối

Để triển khai Office 365 ProPlus trên một máy chủ Windows bằng cách sử dụng dịch vụ máy tính để bàn từ xa (RDS), tên cũ là dịch vụ đầu cuối:
  
- Bạn phải có một kế hoạch Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc doanh nghiệp E5. Các gói Office 365 Business và Office 365 doanh nghiệp bảo hiểm không bao gồm Office 365 ProPlus.
    
- Bạn cần cho phép [dùng chung máy tính kích hoạt](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ cổng Office 365, ** *sử dụng thiết lập cài đặt mặc định* **, hãy làm theo các bước sau: 
  
1. Kiểm tra những gì kế hoạch Office 365 bạn có. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Nếu cần thiết, chuyển sang một khác nhau Office 365 có kế hoạch. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Nếu văn phòng đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch nào khác của Office 365, gỡ bỏ cài đặt nó. Ví dụ, bằng cách vào Control Panel \> gỡ bỏ cài đặt một chương trình. Gỡ cài đặt bằng cách sử dụng [Microsoft hỗ trợ và phục hồi chương trình hỗ trợ](https://aka.ms/SARA-OfficeUninstall-Alchemy) nếu bạn đang chạy vào các vấn đề. 
    
4. Trên máy chủ RDS, đăng nhập vào cổng Office 365 với tài khoản quản trị của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Sau khi văn phòng được cài đặt, ** *không mở hoặc đăng nhập* ** cho bất kỳ ứng dụng văn phòng. 
    
6. Trên máy chủ RDS, cho phép dùng chung máy tính kích hoạt bằng cách chỉnh sửa đăng ký bằng cách làm theo các bước sau:
    
1. Nhấp chuột phải vào nút Windows trong thấp hơn ở góc bên trái của màn hình của bạn và chọn Run. Trong các mở hộp, loại **regedit**, và sau đó chọn OK. 
    
2. Chọn có khi được nhắc để cho phép trình biên tập Registry để thay đổi thiết bị của bạn.
    
3. Trong Registry Editor, thêm một chuỗi giá trị của **SharedComputerLicensing** với một thiết lập 1 dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Trên máy chủ RDS, ** *đăng nhập như là một người sử dụng cuối cùng* ** và [xác minh rằng dùng chung máy tính kích hoạt được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn cài đặt và hướng dẫn cài đặt tùy chỉnh bằng cách sử dụng công cụ triển khai văn phòng, hãy xem [Triển khai Office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Để sửa chữa các lỗi liên quan đến dùng chung máy tính kích hoạt, hãy xem [khắc phục sự cố với máy tính được chia sẻ kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

