---
title: Intune Wi-Fi sơ
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
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028252"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi sơ

Việc triển khai thành công Wi-Fi kết nối mạng cho máy khách MDM phụ thuộc vào hồ sơ được triển khai đúng cách phản ánh yêu cầu của cơ sở hạ tầng Wi-Fi công ty. Để xem lại các cài đặt thích hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem mục: 

[Thêm cài Wi-Fi thiết bị chạy Android trong Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Thêm thiết Wi-Fi dành cho Android Enterprise dành riêng và thiết bị được quản lý đầy đủ trong Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Thêm Wi-Fi thiết bị iOS và iPadOS trong Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Thêm Wi-Fi bản cho thiết Windows 10 và mới hơn trong Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Nhập Wi-Fi thiết bị của Windows thiết bị trong Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Sự cố Thường gặp**

**Tôi đang triển khai một hồ Wi-Fi phụ thuộc vào một chứng chỉ đã triển khai được chỉ định trong hồ Wi-Fi bạn. Tuy nhiên, hồ sơ cấu hình đang hiển thị trạng thái lỗi.**

Kiểm tra xem thiết bị của bạn đã nhận được chứng chỉ chưa.

1. Trong Intune, đi tới Tất cả **thiết bị** và chọn thiết bị để > **cấu hình Thiết bị**.

2. Kiểm tra xem tất cả hồ sơ dự kiến đã được liệt kê hay không và ở trạng thái thành công.

3. Đối với hồ sơ Android, nếu bạn có chứng chỉ trung gian trong chuỗi chứng chỉ của mình, hãy đảm bảo chúng được triển khai với các thiết bị Android.

    Để kiểm tra trạng thái chứng chỉ, hãy đi tới Cấu **hình thiết bị**  >  **Cấu hình** của Android Chứng chỉ Thuộc tính  >  **CA**  >  **trung** gian được tin  >  **cậy.**

Nếu bạn tiếp tục thấy lỗi, hãy xem lại các mục quy trình và khắc phục sự cố. Để biết thêm thông tin, hãy [xem mục Tổng quan để khắc phục sự cố hồ sơ chứng chỉ SCEP với Microsoft Intune.](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**Tôi đã triển khai một Wi-Fi sơ cá nhân cho một thiết bị. Intune cho thấy đã thành công, nhưng thiết bị không kết nối Wi-Fi.**

Trạng thái thành công có nghĩa là Intune đã triển khai thành công hồ sơ như được đặt cấu hình. Tuy nhiên, các cấu hình này có thể không khớp với yêu cầu về mạng và/hoặc xác thực của bạn. Để biết thêm chi tiết về kết nối đã thử, hãy xem lại nhật ký trong dịch vụ cơ sở hạ tầng và xác thực (trên Wi-Fi bộ điều khiển điểm Truy nhập và máy chủ NPS/Bán kính). Bạn có thể phải làm việc với nhóm cơ sở hạ tầng mạng hoặc nhà cung cấp cơ sở hạ tầng mạng bên thứ Wi-Fi ba, để thu thập và xem lại các nhật ký.