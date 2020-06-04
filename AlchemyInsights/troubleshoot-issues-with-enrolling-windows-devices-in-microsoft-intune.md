---
title: Khắc phục sự cố với các thiết bị Windows trong Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665854"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Khắc phục sự cố với các thiết bị Windows trong Microsoft InTune

Hãy đánh giá các tài nguyên được liệt kê bên dưới để giải quyết vấn đề của bạn ngay bây giờ.
  
Một số thông báo lỗi phổ biến và giải pháp bước:
  
 **Không thể cài đặt phần mềm, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn. Tải lại gói phần mềm máy khách PC trong bảng điều khiển dành cho quản trị viên. Đánh giá tài liệu này để biết thêm thông tin.
  
 **Mã lỗi 0x801c0003:** Lỗi có thể xảy ra trong các trường hợp sau:
  
-  Người dùng có nhiều thiết bị đăng ký hơn giới hạn thiết bị. Hãy đánh giá các tài liệu này để [xóa thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Người dùng có thể tham gia thiết bị Azure AD" được đặt thành "không." Đặt nó cho tất cả hoặc chọn người dùng. Đánh giá [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) để biết thêm thông tin.

-  Thiết bị đã được đăng ký bởi người dùng khác. Nếu đó là trường hợp, hãy loại bỏ thiết bị khỏi bảng điều khiển Azure InTune hoặc tự hủy đăng ký thiết bị trước khi thử lại.

-  Thiết bị là Windows 10 Home. Chỉ Windows 10 Pro, Education và Enterprise SKUs có thể tham gia Azure Active Directory.

Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
-  Sử dụng [InTune khắc phục sự cố cổng](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết lỗi đăng ký chung. Đánh giá [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) để biết thêm chi tiết.

-  Đánh giá các tài liệu này để biết danh sách các lỗi phổ biến ngăn đăng ký và giải pháp cho từng: [hướng dẫn khắc phục sự cố](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) và [gỡ rối doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Tìm hiểu cách đăng ký thiết bị Windows trong Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
