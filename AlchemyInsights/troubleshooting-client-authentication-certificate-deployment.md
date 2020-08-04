---
title: Khắc phục sự cố triển khai chứng chỉ xác thực máy khách
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555804"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Khắc phục sự cố triển khai chứng chỉ xác thực máy khách

InTune NDES/SCEP và PKCS/PFX hồ sơ chứng chỉ máy khách thường được sử dụng kết hợp với các loại hồ sơ khác như WiFi, VPN và email cho phép người dùng xác thực với tài nguyên của công ty. Khi các loại hồ sơ được liên kết với hồ sơ chứng chỉ máy khách phụ thuộc vào việc triển khai thành công hồ sơ đó.

Thiết lập cơ sở hạ tầng ban đầu và cấu hình liên quan của hồ sơ chứng chỉ máy khách thường yêu cầu khắc phục sự cố. Để có hướng dẫn từng bước để thiết lập thành công kết nối NDES và khắc phục sự cố hướng dẫn để tách các vấn đề với triển khai chứng chỉ, hãy xem: 

- [Cấu hình cơ sở hạ tầng để hỗ trợ SCEP với InTune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Tổng quan về khắc phục sự cố cấu hình chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Sử dụng tập lệnh PowerShell tham chiếu để giúp xác minh cấu hình của bạn. Để biết thêm thông tin, xem [tập lệnh xác minh kết nối chứng chỉ InTune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Các vấn đề thường gặp khác**

**Khi tôi cố gắng cài đặt kết nối InTune chứng chỉ trên máy chủ kết nối NDES, tôi nhận được thông báo "mật khẩu trong yêu cầu chứng chỉ không được xác minh. Nó có thể đã được sử dụng rồi. Lấy mật khẩu mới để gửi với yêu cầu này. "**  

Thông báo này có nghĩa là bạn cần chạy cài đặt kết nối chứng chỉ là quản trị viên.

Trong một số môi trường, các máy chủ có chạy chứng chỉ InTune phải sử dụng máy chủ proxy để kết nối với InTune, và để kết nối chứng chỉ phải sử dụng proxy. Trong một số trường hợp, kết nối NDES bỏ qua cài đặt proxy được cấu hình và có thể cần thiết để cấu hình thiết đặt ủy quyền trong khi chạy trong ngữ cảnh bảo mật của LocalSystem. 
 
Giải pháp là để chạy Internet Explorer như hệ thống và cấu hình một proxy trong IE. Sau khi khởi động lại dịch vụ InTune Connector, kết nối NDES kết nối với InTune.

**Thiết bị người dùng không còn nhận được chứng chỉ SCEP từ NDES.**

Có thể chứng chỉ xác thực máy khách phát hành cho máy chủ NDES và được chỉ định trong quá trình cài đặt kết nối NDES, đã hết hạn hoặc bị thiếu. Để giải quyết: 
 
1. Dỡ cài đặt kết nối NDES.  
2. Sử dụng các chi tiết để yêu cầu xác thực máy khách mới hoặc chứng chỉ xác thực máy chủ: 
 
    - Tên chủ đề: CN = FQDN bên ngoài  
    - Tên thay thế tiêu đề (cả hai đều bắt buộc): DNS = FQDN bên ngoài, DNS = FQDN nội bộ 
 
3. Cài đặt lại kết nối NDES với chứng chỉ mới.