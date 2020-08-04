---
title: Cấu hình Wi-Fi InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555819"
---
# <a name="intune-wi-fi-profiles"></a>Cấu hình Wi-Fi InTune

Thực hiện thành công kết nối Wi-Fi cho MDM khách hàng phụ thuộc vào một chính xác triển khai hồ sơ phản ánh các yêu cầu của cơ sở hạ tầng Wi-Fi công ty. Để xem lại các cài đặt thích hợp cho các nền tảng máy khách mà bạn đang điều tra: 

[Thêm cài đặt Wi-Fi cho các thiết bị chạy Android trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Thêm cài đặt Wi-Fi cho Android Enterprise chuyên dụng và quản lý toàn bộ thiết bị trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Thêm cài đặt Wi-Fi cho các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Thêm cài đặt Wi-Fi cho Windows 10 và các thiết bị sau trong InTune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Nhập cài đặt Wi-Fi cho các thiết bị Windows trong InTune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Các vấn đề thường gặp**

**Tôi đang triển khai hồ sơ Wi-Fi phụ thuộc vào chứng chỉ đã triển khai được chỉ định trong hồ sơ Wi-Fi. Tuy nhiên, Hồ sơ cấu hình đang hiển thị trạng thái lỗi.**

Kiểm tra xem thiết bị của bạn có nhận chứng chỉ hay không.

1. Trong InTune, đi tới **tất cả thiết bị** và chọn **cấu hình**thiết bị > thiết bị.

2. Kiểm tra tất cả các cấu hình dự kiến được liệt kê và ở trạng thái thành công.

3. Đối với hồ sơ Android, nếu bạn có chứng chỉ trung gian trong Chuỗi chứng chỉ của mình, hãy đảm bảo chúng được triển khai cho các thiết bị Android.

    Để kiểm tra trạng thái chứng chỉ, hãy đi tới **cấu hình thiết bị**  >  **Profiles**  >  **Android trung gian ca**thuộc  >  **tính**  >  **tin cậy chứng chỉ**.

Nếu bạn tiếp tục thấy lỗi, hãy xem lại các quy trình và các phần khắc phục sự cố. Để biết thêm thông tin, xem [tổng quan về khắc phục sự cố cấu hình chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Tôi đã triển khai một cấu hình Wi-Fi cho một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không kết nối với Wi-Fi.**

Trạng thái thành công có nghĩa là InTune đã triển khai thành công hồ sơ dưới dạng cấu hình. Tuy nhiên, các cấu hình có thể không phù hợp với mạng của bạn và/hoặc yêu cầu xác thực. Để biết thêm chi tiết về kết nối cố gắng, kiểm lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên bộ điều khiển điểm truy cập Wi-Fi và máy chủ NPS/Radius). Bạn có thể phải làm việc với nhóm cơ sở hạ tầng mạng của mình hoặc nhà cung cấp Wi-Fi của bên thứ ba để thu thập và đánh giá Nhật ký.