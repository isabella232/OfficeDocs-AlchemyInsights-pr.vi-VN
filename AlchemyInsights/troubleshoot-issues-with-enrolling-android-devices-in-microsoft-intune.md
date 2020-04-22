---
title: Khắc phục sự cố với ghi danh thiết bị Android trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759642"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Khắc phục sự cố với ghi danh thiết bị Android trong Microsoft InTune

Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ.
  
Một số vấn đề thường gặp và các bước giải quyết:
  
 **Thiết bị không được mã hoá lỗi trong cổng công ty:** Các phiên bản Android mới hơn, đặc biệt bắt đầu với v 7.0, yêu cầu mật mã khởi động để đảm bảo rằng thiết bị của bạn được mã hóa hoàn toàn. Các giải pháp phổ biến là kích hoạt pin khởi động hoặc mã hóa đầy đủ thiết bị. Đánh giá [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) để biết thêm thông tin.
  
 **Thiết bị không thể kiểm tra với dịch vụ InTune hoặc hiển thị là "không lành mạnh" trong bảng điều khiển quản trị InTune:** Một số thiết bị Samsung 4,4 và 5,5 có thể không kiểm tra vào dịch vụ. Có 3 giải pháp có thể cho vấn đề này:
  
1. Mở thủ công ứng dụng cổng thông tin công ty InTune, sẽ tự động khởi tạo đồng bộ hóa thiết bị.

2. Cập Nhật thiết bị lên Android 6,0 trở lên.

3. Vô hiệu hoá Samsung Smart Manager từ quản lý cổng thông tin công ty InTune. Xem lại [tài liệu này](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) để biết thêm chi tiết về các vấn đề và nghị quyết.

 **Người dùng loại giấy phép không hợp lệ** hoặc **tên người dùng không được nhận dạng lỗi:** người dùng cần được gán một giấy phép InTune hoặc EMS. Đánh giá các tài liệu này để gán giấy phép thông qua: Trung tâm quản trị văn phòng hoặc cổng thông tin Azure.
  
Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
1. Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung. Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

2. Đánh giá [tài liệu này](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) để biết danh sách các lỗi phổ biến ngăn chặn đăng ký và giải pháp cho mỗi.

3. [Tìm hiểu cách đăng ký thiết bị Android trong Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
