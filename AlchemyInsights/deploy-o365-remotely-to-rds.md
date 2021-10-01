---
title: Triển khai Ứng dụng Microsoft 365 dùng chung trên RDS, Máy chủ Đầu cuối hoặc VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077272"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Triển khai Ứng dụng Microsoft 365 dùng chung trên RDS, Máy chủ Đầu cuối hoặc VDI

Để triển khai Ứng dụng Microsoft 365 dụng Dịch vụ Máy tính Từ xa (RDS), trước đây là Dịch vụ Thiết bị Đầu cuối, bạn phải:

- Sử dụng bản sửa lỗi dễ dàng để bật TLS 1.2 làm mặc định nếu bạn đang chạy phiên bản cũ hơn của Windows (ví dụ: Windows 7 SP1, Windows Server 2008 R2). Để dễ dàng sửa lỗi và biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)làm giao thức bảo mật mặc định trong WinHTTP trong Windows. 
- Có kế hoạch bao gồm Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn (trước đây là Office 365 Plus). Ví dụ: Office 365 E3 hoặc Microsoft 365 E5 hoặc bất kỳ gói nào bao gồm phiên bản Project hoặc Visio trên máy tính, như Gói Project 3 hoặc Gói Visio 2 hay gói Microsoft 365 Business Premium, cũng bao gồm bản Ứng dụng Microsoft 365 dành cho doanh nghiệp.
- Bật kích hoạt máy tính dùng chung. Để biết thêm thông tin, xem [mục Tổng quan về kích hoạt máy tính dùng chung Ứng dụng Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Lưu ý:** Để cài đặt Ứng dụng Microsoft 365 ở chế độ kích hoạt máy tính dùng chung, hãy tải xuống và [chạy Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ.](https://aka.ms/SaRA_OfficeSCA_M365Portal) Để biết chi tiết về các điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn để tùy chỉnh các bản cài đặt bằng cách sử dụng Công cụ Triển khai Office, hãy xem Triển khai [Ứng dụng Microsoft 365](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)bằng cách sử dụng Dịch vụ Máy tính Từ xa .

Để khắc phục các lỗi liên quan đến việc kích hoạt máy tính dùng chung, hãy xem:

- [Khắc phục sự cố với việc kích hoạt máy tính dùng chung Ứng dụng Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Đặt lại Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn thái kích hoạt](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Nếu bạn muốn cài đặt Ứng dụng Microsoft 365 RDS từ Trung Trung tâm quản trị Microsoft 365 sử dụng cài đặt mặc định, hãy làm theo các bước sau:

1. Kiểm tra xem Microsoft 365 bạn có gói nào. Để biết thêm thông tin, [hãy xem Tôi có đăng ký nào?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Nếu cần, hãy chuyển sang gói Microsoft 365 khác. Để biết thêm thông tin, [hãy xem nâng cấp lên gói khác](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Nếu máy Ứng dụng Microsoft 365 đã được cài đặt trên máy chủ RDS bằng bất kỳ gói nào khác không tương thích, hãy gỡ cài đặt nó bằng cách đi tới Gỡ cài đặt một chương trình **trong Panel** Điều  >  **khiển**. Nếu bạn gặp sự cố, hãy gỡ cài đặt bằng cách [tải xuống Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Trên máy chủ RDS, đăng nhập vào trang web bằng Trung tâm quản trị Microsoft 365 quản trị viên của bạn và [cài đặt Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Sau khi Office được cài đặt, đừng mở hoặc đăng nhập vào bất kỳ ứng Office nào.

1. Trên máy chủ RDS, bật kích hoạt máy tính dùng chung bằng cách chỉnh sửa sổ đăng ký:

   1. Bấm chuột phải vào Windows Màn hình ở góc dưới bên trái màn hình, rồi chọn **Chạy**. Trong hộp Mở, nhập **regedit**, sau đó chọn **OK**.

   1. Khi được nhắc cho phép Trình soạn thảo Sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn, hãy **chọn Có**.

   1. Trong Trình soạn thảo Sổ đăng ký, dưới HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, thêm giá trị chuỗi của **SharedComputerLicensing** với cài **đặt là 1.**

1. Trên máy chủ RDS, đăng nhập với tư cách người dùng cuối và xác minh rằng kích hoạt máy tính dùng chung được bật cho người Ứng dụng Microsoft 365. 

   Để biết chi tiết, hãy xem Xác nhận rằng tính năng kích hoạt máy tính [dùng chung đã được Ứng dụng Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)