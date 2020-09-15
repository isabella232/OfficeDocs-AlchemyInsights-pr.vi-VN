---
title: Khắc phục sự cố triển khai chứng chỉ xác thực khách
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659008"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Khắc phục sự cố triển khai chứng chỉ xác thực khách

InTune NDES/SCEP và PKCS/PFX Client, Hồ sơ chứng chỉ được sử dụng thường xuyên cùng với các kiểu hồ sơ khác chẳng hạn như WiFi, VPN và email để cho phép người dùng xác thực đối với tài nguyên của công ty. Khi các kiểu hồ sơ này được nối kết với hồ sơ chứng chỉ máy khách sẽ phụ thuộc vào việc triển khai thành công hồ sơ đó.

Thiết lập cơ sở hạ tầng ban đầu và cấu hình liên kết của hồ sơ chứng chỉ máy khách thường bắt buộc khắc phục sự cố. Để có hướng dẫn từng bước để thiết lập thành công của trình kết nối NDES và hướng dẫn khắc phục sự cố để tách biệt các vấn đề với triển khai chứng chỉ, hãy xem: 

- [Cấu hình cơ sở hạ tầng để hỗ trợ SCEP bằng InTune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Tổng quan về khắc phục sự cố các hồ sơ chứng chỉ SCEP với Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Sử dụng các tập lệnh PowerShell được tham chiếu để giúp xác minh cấu hình của bạn. Để biết thêm thông tin, hãy xem [script xác minh trình kết nối InTune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Các vấn đề phổ biến khác**

**Khi tôi tìm cách cài đặt trình kết nối chứng chỉ InTune trên máy chủ kết nối NDES, tôi nhận được thông báo, "mật khẩu trong yêu cầu chứng chỉ không thể được xác nhận. Có thể nó đã được sử dụng. Lấy mật khẩu mới để gửi yêu cầu này. "**  

Thông báo này có nghĩa là bạn cần chạy cài đặt trình kết nối chứng chỉ với tư cách là người quản trị.

Trong một số môi trường, các máy chủ có chứng chỉ InTune chạy phải sử dụng máy chủ proxy để kết nối với InTune, và vì vậy trình kết nối chứng chỉ phải sử dụng proxy. Trong một số trường hợp, đường kết nối NDES bỏ qua thiết đặt proxy được cấu hình và có thể là cần thiết để cấu hình các thiết đặt proxy trong khi đang chạy trong ngữ cảnh bảo mật của LocalSystem. 
 
Giải pháp là chạy Internet Explorer dưới dạng hệ thống và đặt cấu hình proxy trong IE. Sau khi khởi động lại dịch vụ kết nối InTune, đường kết nối NDES sẽ kết nối đến InTune.

**Thiết bị người dùng không còn nhận được chứng chỉ SCEP từ NDES.**

Có thể là chứng chỉ xác thực máy khách đã phát hành với máy chủ NDES và đã xác định trong quá trình cài đặt kết nối NDES, đã hết hạn hoặc bị thiếu. Để giải quyết: 
 
1. Gỡ cài đặt trình kết nối NDES.  
2. Sử dụng các chi tiết này để yêu cầu chứng chỉ xác thực máy khách mới hoặc chứng thực máy chủ: 
 
    - Tên chủ đề: CN = bên ngoài FQDN  
    - Chủ đề tên thay thế (cả hai đều bắt buộc): DNS = bên ngoài FQDN, DNS = FQDN nội bộ 
 
3. Cài đặt lại trình kết nối NDES với chứng chỉ mới.