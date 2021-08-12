---
title: Sự cố liên quan đến VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971001"
---
# <a name="vpn-related-issues"></a>Sự cố liên quan đến VPN

Việc triển khai thành công khả năng kết nối VPN cho máy khách MDM phụ thuộc vào hồ sơ được triển khai phản ánh đúng các yêu cầu của cơ sở hạ tầng VPN. Để biết các cài đặt thích hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem mục: 

[Windows 10 các cài Windows Ba chiều để thêm kết nối VPN bằng Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Thêm cài đặt VPN trên thiết bị iOS và iPadOS trong Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Cài đặt thiết bị Android để đặt cấu hình VPN trong Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Thêm cài đặt VPN trên thiết bị macOS trong Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Nếu hồ sơ VPN của bạn sử dụng xác thực dựa trên chứng chỉ, hãy đảm bảo rằng hồ sơ chứng chỉ gốc và chứng chỉ xác thực khách được liên kết với hồ sơ VPN đều được triển khai thành công.

**Sự cố Thường gặp**

**Tôi đã triển khai cấu hình VPN cho một thiết bị. Intune cho thấy đã thành công, nhưng thiết bị không kết nối với VPN.**

Trạng thái thành công có nghĩa là Intune đã triển khai thành công hồ sơ như được đặt cấu hình. Tuy nhiên, các cấu hình này có thể không khớp với yêu cầu về mạng và/hoặc xác thực của bạn. Xem lại nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên máy chủ VPN và máy chủ NPS/Bán kính) để biết thêm chi tiết về kết nối đã thử. Bạn có thể cần làm việc với nhóm cơ sở hạ tầng mạng hoặc nhà cung cấp VPN bên thứ ba để thu thập và xem lại nhật ký.

**Khi tôi đặt cấu hình một VPN tùy chỉnh cho iOS, tính năng VPN cho mỗi ứng dụng sẽ không sẵn dùng.**

VPN cho mỗi ứng dụng cho các thiết bị iOS trong Intune hiện sẵn dùng cho một danh sách cụ thể các nhà cung cấp và đối tác, những người cũng phải đáp ứng các điều kiện tiên quyết của chứng chỉ trước khi đặt cấu hình VPN cho mỗi ứng dụng. Để biết thêm thông tin, xem mục Thiết lập Mạng Riêng Ảo (VPN) cho các thiết bị [iOS/iPadOS trong Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Để biết thêm thông tin về tất cả các loại kết nối VPN trong Intune, xem mục Tạo cấu hình VPN để kết nối với [máy chủ VPN trong Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN Theo Yêu cầu của iOS không kích hoạt khi một miền được đặt cấu hình được truy nhập**

Để kiểm tra cài đặt VPN tự động, hãy đặt các giá trị sau:

Tôi muốn thực hiện như sau: Đánh giá **mỗi lần thử kết nối** 

Chọn có kết nối không: **kết Kết nối nếu cần**

Khi người dùng truy nhập những tên miền này: **tên** *miền đích*

Nếu cấu hình ở trên không thành công, hãy thêm thành phần sau đây:

Khi URL này không thể tiếp cận, hãy buộc kết nối VPN: **BADURL**