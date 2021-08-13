---
title: Triển khai ứng dụng Intune Win32
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
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925907"
---
# <a name="intune-win32-app-deployment"></a>Triển khai ứng dụng Intune Win32

Microsoft Intune phép các ứng dụng Win32, bao gồm nhưng không giới hạn ở MSI và .EXE sẽ được triển khai cho tất cả các Windows 10 của bạn. Cơ chế triển khai được sử dụng yêu cầu Phần mở rộng Quản lý Intune (IME) xuất hiện trên thiết bị đích. IME sẽ được cài đặt tự động do việc nhắm tới tập lệnh powershell hoặc triển khai ứng dụng win32 cho người dùng / thiết bị.

Ngoài ra, còn có một số điều kiện tiên quyết cần phải đáp ứng để triển khai các ứng dụng Win32, trong đó bao gồm:

- Nền tảng được hỗ trợ: Windows 10 bản 1607 trở lên (phiên bản Enterprise, Pro và Education).
- Kiến trúc được hỗ trợ: x86 và x64.
- Quản lý Thiết bị: AAD đã kết nối và đăng ký tự động (bao gồm miền kết hợp đã gia nhập và chính sách nhóm đã tự động đăng ký).
- Định dạng Gói Ứng dụng: . **tệp intunewin** do công cụ Chuẩn bị [nội dung Microsoft Win32 chuẩn bị.](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)
- Giới hạn:
    - Kích cỡ tối đa: 8GB.
    - Kiến trúc không được hỗ trợ: ARMs.

Xem lại tài liệu " Thêm, gán và giám sát ứng dụng[Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)trong Microsoft Intune " để biết thông tin liên quan đến các bước đó.

Chi tiết về cách khắc phục sự cố triển khai ứng Windows bao gồm các ứng dụng Win32 có thể được xem lại trong các tài liệu sau

- [Khắc phục sự cố Cài đặt Ứng dụng](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Khắc phục sự cố ứng dụng Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)