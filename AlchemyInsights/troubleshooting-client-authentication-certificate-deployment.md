---
title: Khắc phục sự cố triển khai chứng chỉ Xác thực Máy khách
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020826"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Khắc phục sự cố triển khai chứng chỉ Xác thực Máy khách

Hồ sơ chứng chỉ máy khách NDES/SCEP và PKCS/PFX của Intune thường được sử dụng kết hợp với các loại hồ sơ khác như Wifi, VPN và email để cho phép người dùng xác thực với tài nguyên công ty. Khi các loại hồ sơ đó được nối kết với hồ sơ chứng chỉ máy khách sẽ phụ thuộc vào việc triển khai thành công hồ sơ đó.

Thiết lập cơ sở hạ tầng ban đầu và cấu hình liên kết của hồ sơ Chứng chỉ Máy khách thường yêu cầu khắc phục sự cố. Để xem hướng dẫn từng bước về việc thiết lập thành công bộ nối NDES và hướng dẫn khắc phục sự cố để cách ly các sự cố với việc triển khai chứng chỉ, hãy xem: 

- [Đặt cấu hình cơ sở hạ tầng để hỗ trợ SCEP với Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Tổng quan về cách khắc phục sự cố hồ sơ chứng chỉ SCEP với Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Sử dụng tập lệnh powershell được tham chiếu để giúp xác minh cấu hình của bạn. Để biết thêm thông tin, hãy xem [intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Các sự cố phổ biến khác**

**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. Số này có thể đã được sử dụng. Nhận mật khẩu mới để gửi yêu cầu này."**  

This message means that you need to run the certificate connector installation as an Administrator.

In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy. Trong một số trường hợp, Bộ nối NDES bỏ qua thiết đặt proxy được cấu hình và có thể cần phải cấu hình thiết đặt proxy trong khi đang chạy trong ngữ cảnh bảo mật của LocalSystem. 
 
Giải pháp là chạy Internet Explorer dưới dạng HỆ THỐNG và cấu hình proxy trong IE. Sau khi khởi động lại Dịch vụ Trình kết nối Intune, Trình kết nối NDES sẽ kết nối với Intune.

**Thiết bị người dùng không còn nhận được chứng chỉ SCEP từ NNDES nữa.**

Có thể chứng chỉ Xác thực Máy khách được cấp cho máy chủ NDES và được chỉ định trong quá trình cài đặt bộ nối NDES đã hết hạn hoặc bị thiếu. Để giải quyết: 
 
1. Gỡ cài đặt bộ nối NDES.  
2. Use these details to request a new client authentication or server authentication certificate: 
 
    - Tên chủ đề: CN=fqdn bên ngoài  
    - Tên thay thế chủ đề (cả hai đều là bắt buộc): DNS=fqdn bên ngoài, DNS=fqdn nội bộ 
 
3. Cài đặt lại bộ nối NDES với chứng chỉ mới.