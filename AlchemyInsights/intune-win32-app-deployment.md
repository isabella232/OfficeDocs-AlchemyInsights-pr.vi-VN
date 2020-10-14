---
title: Triển khai ứng dụng InTune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461998"
---
# <a name="intune-win32-app-deployment"></a>Triển khai ứng dụng InTune Win32

Microsoft InTune cho phép các ứng dụng Win32, bao gồm nhưng không giới hạn đối với MSI và. EXE sẽ được triển khai cho các thiết bị chạy Windows 10. Cơ chế triển khai dùng yêu cầu phần mở rộng quản lý InTune (IME) sẽ được trình bày trên thiết bị đích. IME sẽ được cài đặt tự động như là kết quả của việc nhắm vào một tập lệnh PowerShell hoặc triển khai ứng dụng Win32 cho người dùng/thiết bị.

Ngoài ra còn có một tập hợp các site Pre-requiphải được đáp ứng để triển khai các ứng dụng Win32, trong đó bao gồm:

- Nền tảng được hỗ trợ: Windows 10 phiên bản 1607 trở lên (các phiên bản Enterprise, Pro và Education).
- Kiến trúc được hỗ trợ: x86 và x64.
- Quản lý thiết bị: đã tham gia và tự động đăng ký (bao gồm cả tên miền hỗn hợp gia nhập và tự động đăng ký cho chính sách Nhóm).
- Định dạng gói ứng dụng:. tệp **intunewin**  được chuẩn bị bởi [công cụ Prep Microsoft Win32 Content](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Ể
    - Kích cỡ tối đa: 8GB.
    - Cấu trúc không được hỗ trợ: cánh tay.

Xem lại tài liệu "[Thêm, gán và theo dõi ứng dụng Win32 trong Microsoft InTune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" để biết thông tin liên quan đến các bước sau.

Chi tiết về khắc phục sự cố về triển khai ứng dụng trên Windows bao gồm các ứng dụng Win32 có thể được xem xét trong các tài liệu sau đây

- [Khắc phục sự cố cài đặt ứng dụng](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Khắc phục sự cố ứng dụng Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)