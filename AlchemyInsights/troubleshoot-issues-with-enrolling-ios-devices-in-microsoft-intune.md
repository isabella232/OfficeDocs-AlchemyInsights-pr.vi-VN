---
title: Khắc phục sự cố với ghi các thiết bị iOS trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736180"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Khắc phục sự cố với ghi các thiết bị iOS trong Microsoft InTune

Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ. 
  
Một số thông báo lỗi phổ biến và giải pháp bước:
  
- **Thiết bị Cap đạt** Người dùng có nhiều thiết bị đăng ký hơn giới hạn thiết bị. Hãy đánh giá các tài liệu này để [xóa thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Dịch vụ này không được hỗ trợ. Không có chính sách đăng ký:** dịch vụ thông báo đẩy của Apple (APNS) cần phải được cấu hình hoặc gia hạn. Đánh giá [tài liệu này](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) để biết hướng dẫn về cách thực hiện điều đó. 
    
- **Người dùng loại giấy phép không hợp lệ hoặc tên người dùng không được công nhận:** Người dùng cần được gán giấy phép InTune hoặc EMS. Đánh giá các tài liệu này để gán giấy phép thông qua: [Trung tâm quản trị văn phòng](https://docs.microsoft.com/intune/licenses-assign) hoặc [cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
1. Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung. Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết. 
    
2. Đánh giá các tài liệu này để biết danh sách các lỗi phổ biến ngăn đăng ký và giải pháp cho từng: [hướng dẫn khắc phục sự cố](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) và [gỡ rối doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Tìm hiểu cách đăng ký thiết bị iOS trong Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

