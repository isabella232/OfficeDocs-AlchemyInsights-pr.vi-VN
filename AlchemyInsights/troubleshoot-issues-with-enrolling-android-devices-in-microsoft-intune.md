---
title: Gỡ rối các vấn đề với đăng ký các thiết bị Android trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420614"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Gỡ rối các vấn đề với đăng ký các thiết bị Android trong Microsoft Intune

Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.
  
Một số vấn đề thường gặp và các bước giải quyết:
  
 **Thiết bị không mã hóa lỗi vào cổng thông tin công ty:** Các phiên bản mới hơn của Android, đặc biệt là bắt đầu với v7.0, yêu cầu mã khóa khởi động để đảm bảo rằng thiết bị của bạn đã được mã hóa hoàn toàn. Giải pháp phổ biến là để kích hoạt một pin khởi động hoặc đầy đủ mã hóa thiết bị. Xem lại [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) cho biết thêm thông tin. 
  
 **Thiết bị không kiểm tra tại với các dịch vụ dành hoặc hiển thị là "Không lành mạnh" trong giao diện điều khiển admin dành:** Một số 4,4 Samsung và các thiết bị 5.5 có thể không đánh dấu vào dịch vụ. 3 các giải pháp cho vấn đề này có: 
  
1. Tự mở ứng dụng cổng thông tin công ty dành, sẽ tự động bắt đầu một đồng bộ thiết bị.
    
2. Cập nhật các thiết bị Android 6.0 hoặc cao hơn.
    
3. Vô hiệu hóa Samsung Smart Manager quản lý cổng thông tin công ty dành. Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) cho biết thêm chi tiết về các vấn đề và độ phân giải. 
    
 **Không hợp người dùng giấy phép loại lệ** hoặc **dùng tên không công nhận lỗi:** người sử dụng cần phải được gán một giấy phép dành hoặc EMS. Xem xét các tài liệu này để gán một giấy phép thông qua: Cổng thông tin Trung tâm quản trị văn phòng hoặc Azure. 
  
Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
1. Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết. 
    
2. Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi. 
    
3. [Tìm hiểu làm thế nào để đăng ký các thiết bị Android trong Microsoft dành](https://docs.microsoft.com/intune/android-enroll).
    

