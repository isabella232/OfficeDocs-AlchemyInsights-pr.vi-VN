---
title: Khắc phục sự cố với các thiết bị đăng ký Windows trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658900"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Khắc phục sự cố với các thiết bị đăng ký Windows trong Microsoft InTune

Xem lại các tài nguyên được liệt kê dưới đây để giải quyết sự cố của bạn ngay bây giờ.
  
Một số thông báo lỗi và giải pháp thông thường:
  
 **Không thể cài đặt phần mềm, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn. Tải lại gói phần mềm máy khách PC trong bảng điều khiển quản trị InTune. Xem lại tài liệu này để biết thêm thông tin.
  
 **Mã lỗi 0x801c0003:** Lỗi có thể xảy ra trong các tình huống sau đây:
  
-  Người dùng có thêm các thiết bị được đăng ký với giới hạn của thiết bị. Xem lại các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Người dùng có thể gia nhập các thiết bị cho Azure AD" được đặt là "không". Đặt nó cho tất cả hoặc chọn người dùng. Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) để biết thêm thông tin.

-  Thiết bị này đã được người dùng khác đăng ký. Nếu trường hợp đó, hãy loại bỏ thiết bị khỏi bàn điều khiển Azure InTune hoặc bỏ đăng ký theo cách thủ công thiết bị trước khi thử lại.

-  Thiết bị là Windows 10 Home. Chỉ Windows 10 Pro, Education và Enterprise SKUs có thể gia nhập Azure Active Directory.

Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
-  Sử dụng [cổng thông tin khắc phục sự cố InTune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

-  Xem lại các tài liệu này để biết danh sách các lỗi phổ biến ngăn chặn việc đăng ký và độ phân giải cho từng: [hướng dẫn khắc phục](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) sự cố và trình [xử lý khắc phục sự cố](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Tìm hiểu cách đăng ký thiết bị Windows trong Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
