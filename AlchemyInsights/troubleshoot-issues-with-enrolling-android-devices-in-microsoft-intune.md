---
title: Khắc phục sự cố với các thiết bị Android đăng ký trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689976"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Khắc phục sự cố với các thiết bị Android đăng ký trong Microsoft InTune

Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ.
  
Một số vấn đề và giải pháp thông thường:
  
 **Lỗi thiết bị không được mã hóa trong cổng thông tin công ty:** Các phiên bản Android mới hơn, đặc biệt bắt đầu bằng v 7.0, yêu cầu phải có mã khóa khởi động để đảm bảo rằng thiết bị của bạn đã được mã hóa hoàn toàn. Các giải pháp phổ biến là bật mã pin khởi động hoặc mã hóa đầy đủ thiết bị. Xem lại [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) để biết thêm thông tin.
  
 **Thiết bị không kiểm nhập bằng dịch vụ InTune hoặc hiển thị như "không lành mạnh" trong bảng điều khiển quản trị InTune:** Một số thiết bị Samsung 4,4 và 5,5 có thể không kiểm tra dịch vụ. Có 3 giải pháp có thể xảy ra với sự cố này:
  
1. Mở ứng dụng InTune Company Portal theo cách thủ công, điều này sẽ tự động khởi tạo đồng bộ thiết bị.

2. Cập Nhật thiết bị lên Android 6,0 trở lên.

3. Tắt trình quản lý thông minh Samsung từ quản lý cổng thông tin công ty InTune. Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) để biết thêm chi tiết về các sự cố và độ phân giải này.

 Lỗi **người dùng nhập không hợp lệ** hoặc **tên người dùng không được nhận diện:** người dùng cần phải được giao một giấy phép InTune hoặc EMS. Xem lại các tài liệu này để gán giấy phép thông qua: Trung tâm quản trị Office hoặc cổng thông tin Azure.
  
Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
1. Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

2. Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng người.

3. [Tìm hiểu cách đăng ký thiết bị Android trong Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
