---
title: Gỡ rối các vấn đề với đăng ký thiết bị iOS trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28321226"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Gỡ rối các vấn đề với đăng ký thiết bị iOS trong Microsoft Intune

Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ. 
  
Một số thông báo lỗi phổ biến và các bước giải quyết:
  
- **Điện thoại nắp đạt** Người dùng có thể thêm các thiết bị ghi danh hơn giới hạn của thiết bị. Xem xét các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/en-us/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dịch vụ này không được hỗ trợ. Không có chính sách tuyển sinh:** Apple đẩy thông báo dịch vụ (APNS) cần phải được đặt cấu hình hoặc gia hạn. Xem lại [tài liệu này](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) để được hướng dẫn làm thế nào để làm điều đó. 
    
- **Người dùng giấy phép loại không hợp lệ hoặc không nhận dạng được tên người dùng:** Người dùng cần phải được gán một giấy phép dành hoặc EMS. Xem xét các tài liệu này để gán một giấy phép thông qua: [Trung tâm quản trị văn phòng](https://docs.microsoft.com/en-us/intune/licenses-assign) hoặc [cổng Azure](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
1. Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại. Xem lại [tài liệu này](https://docs.microsoft.com/en-us/intune/help-desk-operators) cho biết thêm chi tiết. 
    
2. Xem xét các tài liệu này cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi: [hướng dẫn giải đáp thắc mắc](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) và [giải đáp thắc mắc doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Tìm hiểu làm thế nào để đăng ký thiết bị iOS trong Microsoft dành](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

