---
title: Các hồ sơ Wi-Fi InTune
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696283"
---
# <a name="intune-wi-fi-profiles"></a>Các hồ sơ Wi-Fi InTune

Việc thực hiện thành công kết nối Wi-Fi cho máy khách MDM tùy thuộc vào một hồ sơ được triển khai chính xác phản ánh các yêu cầu của cơ sở hạ tầng Wi-Fi của công ty. Để xem lại các thiết đặt phù hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem: 

[Thêm thiết đặt Wi-Fi cho các thiết bị chạy Android trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Thêm các thiết đặt Wi-Fi cho thiết bị Android dành riêng và được quản lý đầy đủ trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Thêm thiết đặt Wi-Fi cho các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Thêm thiết đặt Wi-Fi cho Windows 10 và các thiết bị sau này trong InTune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Nhập thiết đặt Wi-Fi cho thiết bị Windows trong InTune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Các sự cố phổ biến**

**Tôi đang triển khai hồ sơ Wi-Fi phụ thuộc vào chứng chỉ được triển khai được xác định trong hồ sơ Wi-Fi. Tuy nhiên, Hồ sơ cấu hình sẽ hiển thị trạng thái lỗi.**

Kiểm tra xem thiết bị của bạn đã nhận được chứng chỉ không.

1. Trong InTune, đi tới **tất cả các thiết bị** và chọn thiết bị > **cấu hình thiết bị**.

2. Kiểm tra xem tất cả hồ sơ dự kiến đều được liệt kê và trong trạng thái thành công.

3. Đối với một hồ sơ Android, nếu bạn có chứng chỉ trung bình trong Chuỗi chứng chỉ, hãy đảm bảo rằng chúng được triển khai cho các thiết bị chạy Android.

    Để kiểm tra trạng thái chứng chỉ, đi tới hồ sơ **cấu hình thiết bị**  >  **Profiles**  >  **Android Trung**bình  >  **tài sản**được  >  **chứng nhận tin cậy**.

Nếu bạn tiếp tục thấy lỗi, hãy xem lại các thủ tục và các phần khắc phục sự cố. Để biết thêm thông tin, hãy xem [tổng quan về khắc phục sự cố các hồ sơ chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Tôi đã triển khai hồ sơ Wi-Fi vào một thiết bị. InTune Hiển thị rằng nó đã thành công nhưng thiết bị không được kết nối với Wi-Fi.**

Trạng thái thành công nghĩa là InTune đã triển khai thành công hồ sơ như được cấu hình. Tuy nhiên, các cấu hình này có thể không khớp với mạng của bạn và/hoặc các yêu cầu xác thực. Để biết thêm chi tiết về kết nối đã thử, hãy xem lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên bộ điều khiển điểm truy nhập Wi-Fi và máy chủ NPS/Radius). Bạn có thể phải làm việc với nhóm cơ sở hạ tầng mạng của bạn hoặc nhà cung cấp Wi-Fi bên thứ ba, để thu thập và xem lại Nhật ký.