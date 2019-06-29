---
title: Gỡ rối các vấn đề với đăng ký thiết bị Windows trong Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353559"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Gỡ rối các vấn đề với đăng ký thiết bị Windows trong Microsoft Intune

Xem xét các nguồn tài nguyên được liệt kê dưới đây để giải quyết vấn đề của bạn bây giờ.
  
Một số thông báo lỗi phổ biến và các bước giải quyết:
  
 **Phần mềm không cần cài đặt, 0x80cf4017:** Chứng chỉ tài khoản của bạn đã hết hạn. Tái tải về gói phần mềm máy tính khách hàng trong giao diện điều khiển Admin dành. Xem lại tài liệu này cho biết thêm thông tin.
  
 **Mã lỗi 0x801c0003:** Các lỗi có thể xảy ra trong các trường hợp sau:
  
1. Người dùng có thể thêm các thiết bị ghi danh hơn giới hạn của thiết bị. Xem xét các tài liệu này để [loại bỏ một thiết bị](https://docs.microsoft.com/intune/devices-wipe) hoặc [thay đổi giới hạn thiết bị](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Người dùng có thể tham gia vào thiết bị để Azure quảng cáo" được thiết lập để "không". Thiết lập nó cho tất cả hoặc chọn người dùng. Xem lại [tài liệu này](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) thêm thông tin.

3. Thiết bị đã được đăng ký bởi người dùng khác. Nếu trường hợp đó xảy ra, loại bỏ các thiết bị từ bàn điều khiển Azure dành hoặc tự unenroll thiết bị trước khi thử lại.

4. Thiết là Windows 10 Home. Chỉ Windows 10 Pro, giáo dục và doanh nghiệp SKUs có thể tham gia vào Azure Active Directory.

Tài nguyên bổ sung để giúp giải quyết vấn đề của bạn:
  
1. Sử dụng [Cổng thông tin khắc phục sự cố dành](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) để chẩn đoán và giải quyết chung đăng ký thất bại. Xem lại [tài liệu này](https://docs.microsoft.com/intune/help-desk-operators) cho biết thêm chi tiết.

2. Xem xét các tài liệu này cho một danh sách các lỗi phổ biến mà ngăn chặn ghi danh và độ phân giải cho mỗi: [hướng dẫn giải đáp thắc mắc](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) và [giải đáp thắc mắc doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Tìm hiểu làm thế nào để đăng ký thiết bị Windows trong Microsoft dành](https://docs.microsoft.com/intune/windows-enroll).
