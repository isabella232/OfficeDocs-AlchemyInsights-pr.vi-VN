---
title: Khắc phục sự cố đăng ký thiết bị Android trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008100"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Khắc phục sự cố đăng ký thiết bị Android trong Microsoft Intune

Xem lại các tài nguyên được liệt kê bên dưới để giải quyết sự cố của bạn ngay.
  
Một số vấn đề thông thường và các bước giải quyết:
  
 **Lỗi Thiết bị không được mã hóa trong Company Portal:** Phiên bản mới hơn của Android, đặc biệt là bắt đầu với v7.0, yêu cầu mật mã khởi động để đảm bảo rằng thiết bị của bạn được mã hóa hoàn toàn. Giải pháp thông thường là cho phép mã pin khởi động hoặc mã hóa hoàn toàn thiết bị. Xem lại [tài liệu này](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) để biết thêm thông tin.
  
 **Các thiết bị không thể kiểm nhập bằng dịch vụ Intune hoặc** hiển thị dưới dạng "Không tốt" trong bảng điều khiển quản trị Intune: Một số thiết bị Samsung 4.4 và 5.5 có thể không kiểm nhập dịch vụ. Có 3 giải pháp khả thi cho vấn đề này:
  
1. Mở ứng dụng Intune Company Portal thủ công, việc này sẽ tự động khởi tạo quá trình đồng bộ thiết bị.

2. Cập nhật thiết bị lên Android 6.0 trở lên.

3. Tắt Samsung Smart Manager khỏi việc quản lý thiết Intune Company Portal. Xem lại [tài liệu này để](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) biết thêm chi tiết về những vấn đề và giải pháp này.

 **Lỗi Loại giấy phép người** dùng Không hợp lệ hoặc Tên Người dùng Không Nhận **dạng:** Người dùng cần được gán giấy phép Intune hoặc EMS. Xem lại các tài liệu này để gán giấy phép thông qua: Trung Office tâm Quản trị hoặc cổng thông tin Azure.
  
Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
1. Sử dụng [Cổng thông tin Khắc phục sự cố Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

2. Xem [lại tài liệu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) này để biết danh sách các lỗi thường gặp ngăn chặn việc đăng ký và giải pháp cho từng lỗi.

3. [Tìm hiểu cách đăng ký thiết bị Android trong Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
