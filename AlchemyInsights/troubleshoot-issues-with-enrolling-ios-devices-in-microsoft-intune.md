---
title: Khắc phục sự cố với các thiết bị đăng ký iOS trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669270"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Khắc phục sự cố với các thiết bị đăng ký iOS trong Microsoft InTune

Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ. 
  
Một số thông báo lỗi và giải pháp thông thường:
  
- **Nắp thiết bị đã đạt** Người dùng có thêm các thiết bị được đăng ký với giới hạn của thiết bị. Xem lại các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dịch vụ này không được hỗ trợ. Không có chính sách đăng ký:** dịch vụ thông báo đẩy táo (APNS) cần được cấu hình hoặc gia hạn. Xem lại [tài liệu này](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) để biết hướng dẫn về cách thực hiện điều đó. 
    
- **Loại giấy phép người dùng không được nhận diện không hợp lệ hoặc tên người dùng:** Người dùng cần được gán giấy phép InTune hoặc EMS. Xem lại các tài liệu này để gán giấy phép thông qua: [Trung tâm quản trị Office](https://docs.microsoft.com/intune/licenses-assign) hoặc [cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
1. Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết. 
    
2. Xem lại các tài liệu này để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng: [hướng dẫn khắc phục](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) sự cố và trình [xử lý khắc phục sự cố](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Tìm hiểu cách đăng ký thiết bị iOS trong Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

