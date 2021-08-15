---
title: Khắc phục sự cố đăng ký thiết Windows thiết bị trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981063"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Khắc phục sự cố đăng ký thiết Windows thiết bị trong Microsoft Intune

Xem lại các tài nguyên được liệt kê bên dưới để giải quyết sự cố của bạn ngay.
  
Một số thông báo lỗi phổ biến và các bước giải quyết:
  
 **Không cài đặt được phần mềm, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn. Tải xuống lại gói phần mềm Máy khách PC trong Bảng điều khiển Quản trị Intune. Xem lại tài liệu này để biết thêm thông tin.
  
 **Mã lỗi sẽ 0x801c0003:** Lỗi này có thể xảy ra trong các kịch bản sau đây:
  
-  Người dùng có nhiều thiết bị đã đăng ký hơn giới hạn thiết bị. Xem lại các tài liệu này [để loại bỏ một thiết](https://docs.microsoft.com/intune/devices-wipe) bị hoặc thay đổi giới hạn thiết [bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Người dùng có thể liên kết thiết bị với Azure AD" được đặt là "không có". Đặt thành tất cả hoặc chọn người dùng. Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) để biết thêm thông tin.

-  Thiết bị này đã được đăng ký bởi một người dùng khác. Nếu vậy, hãy loại bỏ thiết bị khỏi bảng điều khiển Azure Intune hoặc bỏ kiểm soát thủ công thiết bị trước khi thử lại.

-  Thiết bị đã được Windows 10 Home. Chỉ các S WINDOWS 10 PRO, Giáo dục và Doanh nghiệp mới có thể gia nhập một Azure Active Directory.

Các tài nguyên bổ sung để giúp giải quyết sự cố của bạn:
  
-  Sử dụng [Cổng thông tin Khắc phục sự cố Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết các lỗi đăng ký thường gặp. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

-  Xem lại các tài liệu này để biết danh sách các lỗi thường gặp ngăn chặn việc đăng ký và giải pháp cho mỗi lỗi: Hướng dẫn [khắc](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) phục sự cố và [tài liệu Khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Tìm hiểu cách đăng ký thiết Windows thiết bị trong Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
