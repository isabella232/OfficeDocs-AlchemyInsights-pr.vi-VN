---
title: Khắc phục sự cố đăng ký thiết bị iOS trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047998"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Khắc phục sự cố đăng ký thiết bị iOS trong Microsoft Intune

Xem lại các tài nguyên được liệt kê bên dưới để giải quyết sự cố của bạn ngay. 
  
Một số thông báo lỗi phổ biến và các bước giải quyết:
  
- **Đã đạt Đến Hạn mức Thiết bị** Người dùng có nhiều thiết bị đã đăng ký hơn giới hạn thiết bị. Xem lại các tài liệu này [để loại bỏ một thiết](https://docs.microsoft.com/intune/devices-wipe) bị hoặc thay đổi giới hạn thiết [bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dịch vụ này không được hỗ trợ. Không có Chính sách Đăng ký:** Cần cấu hình hoặc gia hạn Dịch vụ Thông báo Đẩy (APNS) của Apple. Xem [lại tài liệu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) này để biết hướng dẫn về cách thực hiện việc đó. 
    
- **Loại giấy phép người dùng không hợp lệ hoặc tên người dùng không được nhận dạng:** Người dùng cần được gán giấy phép Intune hoặc EMS. Xem lại các tài liệu này để gán giấy phép thông [qua: Trung Office tâm Quản trị](https://docs.microsoft.com/intune/licenses-assign) hoặc cổng thông tin [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
1. Sử dụng [Cổng thông tin Khắc phục sự cố Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết. 
    
2. Xem lại các tài liệu này để biết danh sách các lỗi thường gặp ngăn chặn việc đăng ký và giải pháp cho mỗi lỗi: Hướng dẫn [khắc](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) phục sự cố và [tài liệu Khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Tìm hiểu cách đăng ký thiết bị iOS trong Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

